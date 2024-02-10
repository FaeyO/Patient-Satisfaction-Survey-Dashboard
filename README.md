# Patient Satisfaction Survey Report

### Dashboard Link : https://1drv.ms/x/c/429eb989df50f199/EdUD4CnBGEhLlGDILeMYvoYBtZibXI8b96snAy-l45e4_g?e=lfZhf2

## Problem Statement

This dashboard serves as a pivotal tool for healthcare professionals, facilitating a deeper understanding of their patients' needs and preferences. By leveraging various metrics and ratings, it enables healthcare institutions to gauge the satisfaction levels of their clientele regarding the services provided. Through insightful analysis, it delineates areas warranting enhancement, thereby empowering stakeholders to refine service delivery strategies.

Furthermore, the dashboard provides invaluable insights into key performance indicators such as the average duration of doctor-patient interactions and the typical length of patient stays. Armed with this data, healthcare providers can pinpoint operational inefficiencies and address underlying factors contributing to prolonged wait times or inadequate consultations. This proactive approach enables them to devise targeted interventions aimed at optimizing patient care and operational efficacy.


### Steps followed 

- Step 1 : Load data into Excel Desktop, dataset is a csv file.
- Step 2 : Open excel power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in some of the columns there were errors & empty values adequate data cleaning was carried out.
- Step 5 : In the report view, under the view tab, theme was selected.
- Step 6 : Since the data contains various ratings, the average rating given to the various health facilities were calculated. 
- Step 7 : Visual filters (Slicers) were added for two fields named "Patient Gender", "Year".
- Step 8 : A bar chart was also added to the report design area representing the number of satisfied & neutral/unsatisfied customers. While creating this visual, field named "Gender" was also added to the Legends bucket, thus number of customers are also seggregated according the gender. 
- Step 9 : Various  Visual like pie charts, bar charts, bullet chart was used to show the different ratings given to the various health failities on average on the criteria mentioned below,

  (a) Patient Length of stay

  (b) Amount of time spent with doctor
  
  (c) Overall care provided at a medical facility
  
  (d) Likeliness to recommend a medical facility

  (e) How well were treatment and evaluation explained
  
  (f) Overall care provided by medical personnel

- Step 10 : In the report view, under the insert tab, four text boxes were added to the canvas, to show the Total patient who participated in the survey, the number of health facility ,the total distinct count of diagnosis by these patient and the average length of stay of patient.

- Step 11 : In the report view, under the insert tab, using shapes option from elements group a rectangle was inserted & similarly using image option company's logo was added to the report design area. 

- Step 12 : A histogram chart was created to visualize the spread of varoius age of patient who participated in the survey.
        
- Step 13 : New measure was created to find total count of Patients.

Following Excel expression was written for the same,
        
        Total Patient = =COUNTA(Table2[patient_id])
        
A card visual was used to represent count of Patients.

![total_pt_page-0001](https://github.com/FaeyO/Patient-Satisfaction-Survey-Dashboard/assets/118575325/071e352f-65e7-4bf1-a6ba-7cd87b63b2ee)

 - Step 14 : New measure was created to validate the age of patients,
 
 Following EXCEL expression was written to age of patients,
 
         Patients Age =[@[survey_year]]-[@[birth_year]]
 
 An histogram was used to represent the distribution of Age.
 
 ![dist_age_page-0001](https://github.com/FaeyO/Patient-Satisfaction-Survey-Dashboard/assets/118575325/cee242ed-7f00-4ee2-b4dc-afc7ee10650e)
 
 - Step 15 : New measure was created to calculate the year the survey took place.
 
 Following EXCEL expression was written to find year of survey,
 
         survey_year = =LEFT([@[survey_date]],4)

 - Step 16 : The report was then linked to Powerpoint and presented using Powerpoint.
 
# Insights

A single page report was created on Excel Desktop, and the following inferences can be drawn from the dashboard;

### [1] Total Number of Patients = 1047

   Number of Patient (Male) = 488 (46.6 %)

   Number of Patient (Female) = 511 (48.8 %)

   Number of unspecified gender = 48 (4.5 %)

### [2] Average Ratings
    1.)Patient Length of stay
    a) St Mary's Hospital - 14/15
    b) Community HEalth clinic - 17/15
    c)City Medical Center -15/15
    d)Memorial Hospital -15/15
    e) General Hospital -15/15

    2.) Likeliness to recommend a medical facility to friends and family members?
    a) St Mary's Hospital - 5.9/6
    b) Community HEalth clinic - 5.7/6
    c)City Medical Center -5.3/6
    d)Memorial Hospital -5.3/6
    e) General Hospital -5.1/6

    3.) Amount of time spent with doctor
    a) St Mary's Hospital - 5.6/6
    b) Community HEalth clinic - 5.6/6
    c)City Medical Center -5.4/6
    d)Memorial Hospital -5.5/6
    e) General Hospital -5.7/6

    3.) Overall care provided at a medical facility
    a) St Mary's Hospital - 5.9/6
    b) Community HEalth clinic - 5.5/6
    c)City Medical Center -5.7/6
    d)Memorial Hospital -5.8/6
    e) General Hospital -5.7/6

    4.)How well were treatment and evaluation explained
    a) St Mary's Hospital - 5.6/5
    b) Community HEalth clinic - 5.0/5
    c)City Medical Center -5.5/5
    d)Memorial Hospital -5.1/5
    e) General Hospital -5.4/5

    5.)Overall care provided by medical personnel
    a) St Mary's Hospital - 4.3/4
    b) Community HEalth clinic - 3.9/4
    c)City Medical Center -3.9/4
    d)Memorial Hospital -4.3/4
    e) General Hospital -4.0/4

  These ratings will change if different visual filters will be applied.  
  
 ### [3] Some other insights
 
 ### Top 5 discharge depositions
    a)Community Health clinic
    i)ADM
    ii)Expired
    iii)Home
    iv)Inpatient Hospice
    v)Long term care patient

    b)Community Health clinic
    i)ADM
    ii)Expired
    iii)Home
    iv)Court/Law enforcement
    v)Long term care patient

    c)General Hospital
    i)Hospice-Medical facility
    ii)Expired
    iii)Home
    iv)Left Against Medical Advice
    v)Long term care patient

    d)Memorail Hospital
    i)Hospice-Unknown
    ii)Expired
    iii)Home
    v)Long term care patient

    e)St Mary's Hospital
    i)Skilled Nursing facility
    ii)Expired
    iii)Home
    iv)Left Against Medical Advice
    v)Long term care patient


### Dashboard view

![Patient satisfaction survey_ds_page-0001](https://github.com/FaeyO/Patient-Satisfaction-Survey-Dashboard/assets/118575325/14270a7f-6ec6-4697-9700-e76309427ad3)


# Big-Data(Data-Visualization)Project

## Dataset Name: Patient Dataset
## Source: Kaggle
## Description: The dataset provides a detailed breakdown of healthcare services provided in a hospital, including inpatient, outpatient and day case procedures, medical specialties, and patient demographics. 
## The data includes the following information:
Medical Specialties: Specialty HIPE, Specialty Name, Case Type
Patient Demographics: Adult/Child, Age Profile, Time Bands
Procedure Details: Total, Purchase Date, Return Status, Warranty (Months)
The dataset covers various medical specialties, including Neurology, Neurosurgery, Ophthalmology, Orthopedics, Pediatrics, Neonatology, Plastic Surgery, Radiology, Nephrology, Respiratory Medicine, Infectious Diseases, Dental Surgery, and Pediatric Surgery. The data includes the type of procedure (inpatient or outpatient case), the patient's age profile, and the time of day the procedure was performed

## Using DAX function called AVG/MED Wait list. 
    Avg/Med Wait List = SWITCH(VALUES(‘Calculation Method’[Calc Method]), “Average”, [Average Wait List], “Median”, [Median Wait List])
This DAX function calculates average and median of wait list in each medical branch like Neurology, Neurosurgery, Ophthalmology, Orthopedics, etc. Giving a brief idea of how many patients were waiting for the particular branch.

## Using DAX function called Latest Month Wait list.
   Latest Month Wait List = CALCULATE(SUM(All Data[Total]), All Data[Archive Date] = MAX(All Data[Archive Date])) + 0
This DAX function calculates the wait list of the latest month.

## Using DAX function called PY Latest Month Wait list.
     PY Latest Month Wait List = CALCULATE(SUM(All_Data[Total]),All_Data[Archive_Date]= EDATE(MAX(All_Data[Archive_Date]),-12)) + 0
This DAX function calculates the wait list of the latest month.

## Using DAX function called AVG/MED Wait list. 
    Avg/Med Wait List = SWITCH(VALUES(‘Calculation Method’[Calc Method]), “Average”, [Average Wait List], “Median”, [Median Wait List])
This DAX function calculates average and median of wait list in each medical branch like Neurology, Neurosurgery, Ophthalmology, Orthopedics, etc. Giving a brief idea of how many patients were waiting for the particular branch.

## Using DAX function called Latest Month Wait list.
   Latest Month Wait List = CALCULATE(SUM(All Data[Total]), All Data[Archive Date] = MAX(All Data[Archive Date])) + 0
This DAX function calculates the wait list of the latest month.

## Using DAX function called PY Latest Month Wait list.
     PY Latest Month Wait List = CALCULATE(SUM(All_Data[Total]),All_Data[Archive_Date]= EDATE(MAX(All_Data[Archive_Date]),-12)) + 0
This DAX function calculates the wait list of the latest month.

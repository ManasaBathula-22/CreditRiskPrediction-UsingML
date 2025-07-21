# Filename:
Credit Risk Prediction.csv
Records: 30000
Features: 25 (including the target)

# Purpose
This dataset is used to build a credit risk prediction model using customer history over previous 6 months and customer's details like education,gender. Each row represents customer related details as features.

# Key Details:
Target Column: Will_Default_Next_Month
Values: 0 = No, 1 = Yes
Features: 25 numerical columns representing customer history and details, e.g.:
Bill history
Repayment History
Education
Gender
Age 
Credit Limit

# Data Type: 
int32 and int64.

# Missing Values: 
Are in the form of '0'. Replaced them with suitable imputation methods(Median/Mode)

# Modifications Made:
No modifications were made to the original dataset structure.

# Basic preprocessing was performed within the notebook:
Handling Missing Values
Handling Outliers
Feature scaling
Handling Class Imbalance
Splitting data into training and testing sets



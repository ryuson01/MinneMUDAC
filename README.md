# MinneMUDAC 2023
## Predicting MLB Home Game Attendance
MinneAnalytics is host of the annual Midwest Undergraduate Data Analytics Competition; the scope of this year's data science challenge was centered around MLB home game attendance. The sponsor provided The University of Iowa Business Analytics Capstone Group 03-1 with historical Game Log data and previous/upcoming scheduling information, with primary our primary objective being to build a model predictive of MLB home game attendance and understand what aspects of major league baseball games are truly impactful on attendance.

## Getting Started
These instructions will get you a copy of the project up and running on
your local machine for development and testing purposes.
1. Download xxx.rar and extract to desktop
2. Set working directory to folder \Home\ClassData\Marmon 03-1\MLB

### Prerequisites
Items necessary to run this sofware:
1. RStudio Server 2022.07.2 Build 576
2. Packages to install: fastDummies, lubridate, dplyr, randomForest, rpart, caret

### The following scripts broke down tasks for data cleaning, exploratory analysis, and regression modeling.
1. Script 1. MLBscript.R uses inputs
"GameLogs_v2.csv", "OriginalSchedule_v2.csv", "2023_MLBSchedule.csv", and "Minnesota_HomeGames1.csv" 
and produces outputs
"gamelogs_v3.csv", "final_gamelogs.csv", "test_data.csv", "train_data.csv", and "ExDate_GameLog_Subset.csv".

2. Script 2. Regression_Script.R uses inputs
"train_data.csv", "test_data.csv", 
and produces outputs
"rfmodelpred.csv".

3. Script 3. Regression_ExternalData.R uses inputs
"exDa_R2.csv", "GameLogs_v2.csv", and "OriginalSchedule_v2.csv", "2023_MLBSchedule.csv", "Sched23A.csv", "train_data_r2.csv", "test_data_r2.csv
and produces outputs
"gamelogs_r2.csv", "final_gamelogs_r2.csv", "train_data_r2.csv", "ExDate_GameLog_Subset_r2.csv", "test_data_r2.csv", "Sched23_sub.csv", and "rfmodelpred_r2.csv".

4. Script 4. Regression_ExternalData_5years.R uses inputs
"exDa_R2.csv", "GameLogs_v2.csv", "OriginalSchedule_v2.csv", "2023_MLBSchedule.csv", "Sched23A.csv", "train_data_r2.csv", "test_data_r2.csv" 
and produces outputs
"gamelogs_r2.csv", "final_gamelogs_r2.csv", "train_data_r2.csv", "ExDate_GameLog_Subset_r2.csv", "test_data_r2.csv", "Sched23_sub.csv", and "rfmodelpred_5year.csv".

5. Script 5. Regression_ExternalData_DynamicModel.R uses inputs
"exDa_R2.csv", "GameLogs_v2.csv", "OriginalSchedule_v2.csv", "2023_MLBSchedule.csv", "Sched23A.csv", "train_data_r2.csv", "test_data_r2.csv" , "test_data_r3_MIN_rev.csv", "train_data_r3_MIN_rev.csv", "sched23_subset_r3_rev_update.csv"
and produces outputs
"gamelogs_r2.csv", "final_gamelogs_r2.csv", "train_data_r2.csv", "ExDate_GameLog_Subset_r2.csv", "test_data_r2.csv", "Sched23_sub.csv", and "rfmodelpred_r3_update.csv"

## Procedures
1. Upload files from Data folder to R-Studio.
2. Run the MLBscript.R to clean the data and perform a variable importance test. 
3. Run the Regression_Script.R script to determine which regression models performed the best and run initial regression with the original data. 
   - Random Forest, all predictors without cross validation produces the lowest MAE. 
4. Run the Regression_ExternalData.R script to produce attendance predictions with the data set that includes all fo the original inputs along with stadium capacity, city population, number of professional teams in the city, and season. 
5. Run the Regression_ExternalData_5years.R script to produce attendance predictions with the same external inputs as the previous regression model, but the model is now only trained on the previous five years of data. 
6. Run the Regression_ExternalData_DynamicModel.R script to produce attendance predictions for the next Twins home game using the external data along with a column that records the previous home game attendance. 
   - The sched23_subset_r3_rev_update.csv file will need to be updated as more games are played. 
   
## Deployment
This project is not built for deployment.

## Versioning
Version 1.0

## Authors
Beth Tiggelaar
Katie Zawoyski
Sarah Philips
Ryan Yuson

## Acknowledgments
Acknowledgements to Professor Michael Altemeier within The University of Iowa for guidance in modeling, exploration, and analysis 
throughout the the duration of this project.

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
"rfmodelpred.csv" and "cartTunepred.csv".

3. Script 3. Regression2ExDa.R uses inputs
"exDa_R2.csv", "GameLogs_v2.csv", and "OriginalSchedule_v2.csv", "2023_MLBSchedule.csv", "Sched23A.csv", "train_data_r2.csv", "test_data_r2.csv
and produces outputs
"gamelogs_r2.csv", "final_gamelogs_r2.csv", "train_data_r2.csv", "ExDate_GameLog_Subset_r2.csv", "test_data_r2.csv", "Sched23_sub.csv", "rfmodelpred_r2.csv", and "cartTunepred_r2.csv".

4. Script 4. Regression_5years.R uses inputs
"exDa_R2.csv", "GameLogs_v2.csv", "OriginalSchedule_v2.csv", "2023_MLBSchedule.csv", "Sched23A.csv", "train_data_r2.csv", "test_data_r2.csv" 
and produces outputs
"gamelogs_r2.csv", "final_gamelogs_r2.csv", "train_data_r2.csv", "ExDate_GameLog_Subset_r2.csv", "test_data_r2.csv", "Sched23_sub.csv", and "rfmodelpred_r3.csv".

5. Script 5. 

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
Acknowledgements to Professor Michael Altemeier within The University of Iowa for assistance in 
the completion of this projects modeling, exploration, and analysis.

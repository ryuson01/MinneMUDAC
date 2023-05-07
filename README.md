# MinneMUDAC 2023
## Predicting MLB Home Game Attendance
Principal Financial Group of Des Moines has provided The University of
Iowa's Business Analytics Capstone Team 1 with data regarding their stock
trading in order to gain a better understanding of the costs associated
with transactions. The company currently receives data based on 10 curves
from Investment Technology Group (ITG), and estimates transaction costs
based on a linear regression model the company has created. The
Transaction Cost Analysis project purpose is to assist PFG in determining
a more accurate way to estimate stock transaction costs.

## Getting Started
These instructions will get you a copy of the project up and running on
your local machine for development and testing purposes.
1. Download xxx.rar and extract to desktop
2. Set working directory to extracted folder\Data

### Prerequisites
What things you need to run the software
1. R 3.3.2
2. RStudio 1.0.135
3. Packages to install: fastDummies, lubridate, dplyr, randomForest, rpart, caret, .

### Break down into end to end tests
1. Script 1. MLB_Script.R uses inputs
"GameLogs_v2.csv", "OriginalSchedule_v2.csv", "2023_MLBSchedule.csv", and "Minnesota_HomeGames1.csv" and produces outputs "gamelogs_v3.csv",
"final_gamelogs.csv", "test_data.csv", "train_data.csv", and "ExDate_GameLog_Subset.csv".

2. Script 2. Regression_Script.R uses inputs
"train_data.csv", "test_data.csv", and produces outputs "rfmodelpred.csv" and "cartTunepred.csv"

3. Script 3. Regression2ExDa.R uses inputs
"exDa_R2.csv", "GameLogs_v2.csv", and "OriginalSchedule_v2.csv"

4. Script 4. Model-compare ITG v PFG model.R uses inputs
"SmallCap2016.csv", "LargeCap2016.csv", "EM2016.csv",
"SC_stock_list.csv", "LC_stock_list.csv", "EM_stock_list.csv",
"SC_9915US.csv", "LC_4025US.csv", and "EM_4043.csv"

5. Script 5. Model-linear distribution.R uses inputs "SmallCap2016.csv",
"LargeCap2016.csv", "EM2016.csv", "SC_stock_list.csv",
"LC_stock_list.csv", "EM_stock_list.csv", "SC_9915US.csv",
"LC_4025US.csv", and "EM_4043.csv"

6. Script 6. Model-Log.R uses inputs "SmallCap2016.csv",
"LargeCap2016.csv", "EM2016.csv", "SC_stock_list.csv",
"LC_stock_list.csv", "EM_stock_list.csv", "SC_9915US.csv",
"LC_4025US.csv", and "EM_4043.csv"

7. Script 7. Model-Exponential.R uses inputs "SmallCap2016.csv",
"LargeCap2016.csv", "EM2016.csv", "SC_stock_list.csv",
"LC_stock_list.csv", "EM_stock_list.csv", "SC_9915US.csv",
"LC_4025US.csv", and "EM_4043.csv"

8. Script 8. Model-sqrt x.R uses inputs "SmallCap2016.csv",
"LargeCap2016.csv", "EM2016.csv", "SC_stock_list.csv",
"LC_stock_list.csv", "EM_stock_list.csv", "SC_9915US.csv",
"LC_4025US.csv", and "EM_4043.csv" to produce
"LinearErrorbySector.csv"

9. Script 9. Model-sqrt(y) and x.R uses inputs "SmallCap2016.csv",
"LargeCap2016.csv", "EM2016.csv", "SC_stock_list.csv",
"LC_stock_list.csv", "EM_stock_list.csv", "SC_9915US.csv",
"LC_4025US.csv", "EM_4043.csv" to produce output
"LogErrorBySector.csv"

10. Script 10. Model- Error comparison.R uses inputs and code from 9.
Model-sqrt(y) and x.R to product output "PredictionErrorbycurve.csv"
Additional data to upload:
"LinearErrorbySector.csv" "LogErrorBySector.csv"
"PredictionErrorbycurve.csv"

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

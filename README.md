PREDICTORS FOR PHYSICAL HEALTH

#OBJECTIVES
  Do respondents experienced poor phsysical health and for how many days that experience it for in the past 30 days based on the whether they have smoke 100 cigarettes in their entire life, the number of days they drank in the last 30 days and whether or not they have ever had a stroke?
  Determine which predictor or combination of predictors (model) is the better model to predict physical health. The choosen predictors used for this project are , ALCDAY5, SMOKE100 and CVDSTRK3 for PHYSHLTH. 

#DATA SET
[Kaggle](https://www.kaggle.com/cdc/behavioral-risk-factor-surveillance-system)

#LIBRARIES 
library(tidyverse) 
library(caret)

#DATA CLEANING
  Updating data set to only include the variables used.
  Determine and remove outliers from data frame using quantile function within 3 standard deviations of each end of the distribution, using 99.85%  and 0.15% of the upper and lower bounds of each variable. 
  Box plot visualization of outliers within the data. 


# PREDICTORS FOR POOR PHYSICAL HEALTH
> Determining if various predictors contribute to poor physical health utlizing R. 


## Table of Contents
* [Objective](#objective)
* [Dataset Used](#dataset-used)
* [Libraries Used](#libraries-used)
* [Data Cleaning](#data-cleaning)
* [Exploratory Analyses](#exploratory-analyses)
* [Descriptive statistics](#descriptive-statistics)
* [Models](#models)
* [Conclusion](#conclusion)



## Objective
- Using the behavioral-risk-factor-surveillance-system from the CDC, we want to address the following questions. 
- Do respondents experienced poor phsysical health and how many days they experience it for in the past 30 days based on the whether they have smoke 100 cigarettes in their entire life, the number of days they drank in the last 30 days and whether or not they have ever had a stroke?
- Determine which predictor or combination of predictors (model) is the better model to predict physical health. The choosen predictors used for this project are ALCDAY5, SMOKE100 and CVDSTRK3 for PHYSHLTH.


## Dataset Used
- [Kaggle](https://www.kaggle.com/cdc/behavioral-risk-factor-surveillance-system)


## Libraries Used
- tidyverse
- caret


## Data cleaning
-  Updated dataset to only include the variables used
-  Determine and remove outliers from data frame using quantile function within 3 standard deviations of each end of the distribution, using 99.85%       and 0.15% of the upper and lower bounds of each variable
-  Box plot visualization of outliers within the data

<img width="617" alt="Screenshot 2023-12-27 at 4 12 57 PM" src="https://github.com/Navy-Neang/R-programming-project/assets/154766577/7537db7b-eb5e-4d24-acdf-11c90d07e46b">



## Exploratory Analyses
- Exploratory analyses (for each variable) doing appropriate visualizations with ggplot2
<img width="718" alt="Screenshot 2023-12-27 at 4 35 40 PM" src="https://github.com/Navy-Neang/R-programming-project/assets/154766577/96687fd5-09fc-4c6e-8017-6fa7f9868f6c">


## Descriptive statistics
- PHYSHLTH 
  - The variance of this variable is quite high. This tells us that the data is pretty spread out. This finding in the variance is in agreement with the histogram of this variable. You see that      the data is spread out across the range of the dataset. The SD is low, which means that the data are clustered tightly around the mean.
- ALCDAY5
  - The variance of this variable is quite high. This tells us that the data is pretty spread out. This finding in the variance is in agreement with the histogram of this variable. You see that the data is spread out across the range of the dataset. The SD is low, which means that the data are clustered tightly around the mean.
- SMOKE100
  - The variance and SD are both zero, which means that there is essentially there is no spread of the data set and that it is located very tightly around the mean. Since the distribution of those who have and those who havent smoked 100 cigarettes in their entire lives are almost the same, the basic descriptive statistics tells us that there is slightly higher number of those people who have not smoked 100 cigarettes.
- CVDSTRK
  - The variance and SD are both zero, which means that there is essentially there is no spread of the data set and that it is located very tightly around the mean. This means sense since we see that the majority if not all of the respondents did not suffered from a stroke. 


## Models
Model 1 
  - CVDSTRK3 and SMOKE100 predictor combination
  - Linear regression showed positive correlation between the number of days physical health was affected by whether or not the respondent ever suffered from a stroke and those who have and          haven't smoked 100 cigarettes in their entire lives

Model 2 
  - SMOKE100
  - Linear regression showed positive correlation for physical health and smoking


## Conclusion
- Regressions of predictors ( ALCDAY5, SMOKE100 and CVDSTRK3) showed positive correlation for PHYSHLTH
- AIC was used to compare the fit of this regression model vs the other one.
- AIC explains the most variation  in the data, while penalizing the models that use excessive number of parameters.
- The lower the AIC value, the better the model fits. 
- Model 1 performed better than model 2 since it has a lower AIC value




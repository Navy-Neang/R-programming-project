

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

# PREDICTORS FOR PHYSICAL HEALTH
> Determining if various predictors contribute to poor physical health utlizing R. 


## Table of Contents
* [Objective](#objective)
* [Dataset Used](#dataset-used)
* [Libraries used](#libraries)
* [Data Cleaning](#data-cleaning)
* [Data Distribution](#data-distribution)
* [Model](#model)
* [Conclusion](#conclusion)
<!-- * [License](#license) -->


## General Information
- Using the behavioral-risk-factor-surveillance-system from the CDC, we want to address the following questions. 
- Do respondents experienced poor phsysical health and how many days they experience it for in the past 30 days based on the whether they have smoke     100 cigarettes in their entire life, the number of days they drank in the last 30 days and whether or not they have ever had a stroke?
- Determine which predictor or combination of predictors (model) is the better model to predict physical health. The choosen predictors used for this    project are , ALCDAY5, SMOKE100 and CVDSTRK3 for PHYSHLTH.


## Dataset Used
- [Kaggle](https://www.kaggle.com/cdc/behavioral-risk-factor-surveillance-system)


## Libraries Used
- library(tidyverse)
- library(caret)


## Data cleaning
-  Updated dataset to only include the variables used
-  Determine and remove outliers from data frame using quantile function within 3 standard deviations of each end of the distribution, using 99.85%       and 0.15% of the upper and lower bounds of each variable
-  Box plot visualization of outliers within the data
! img width="617" alt="Screenshot 2023-12-27 at 4 12 57 PM" src="https://github.com/Navy-Neang/R-programming-project/assets/154766577/7537db7b-eb5e-4d24-acdf-11c90d07e46b">)
<!-- If you have screenshots you'd like to share, include them here. -->


## Setup
What are the project requirements/dependencies? Where are they listed? A requirements.txt or a Pipfile.lock file perhaps? Where is it located?

Proceed to describe how to install / setup one's local environment / get started with the project.


## Usage
How does one go about using it?
Provide various use cases and code examples here.

`write-your-code-here`


## Project Status
Project is: _in progress_ / _complete_ / _no longer being worked on_. If you are no longer working on it, provide reasons why.


## Room for Improvement
Include areas you believe need improvement / could be improved. Also add TODOs for future development.

Room for improvement:
- Improvement to be done 1
- Improvement to be done 2

To do:
- Feature to be added 1
- Feature to be added 2


## Acknowledgements
Give credit here.
- This project was inspired by...
- This project was based on [this tutorial](https://www.example.com).
- Many thanks to...

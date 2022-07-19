# Exploration Of Intensive Care Unit Data

## Abstract

Data concerning patients admitted to an ICU (Intensive Care Unit) was analysed. It contained among others
information about physiological measurements, diagnosis and outcome.
The data was initially collected from
a database (MIMIC-II) "to investigate the effectiveness of indwelling arterial catheters in hemodynamically stable patients with respiratory failure for mortality outcomes".

First the missing values where analysed and it was investigated if they are missing
in any particular pattern. Exploratory data analysis was done. Pairwise
correlations between the variables where investigated and discussed.
The missing values where imputed using MICE (Multivariate Imputation by Chained Equations).

In order to investigate which of the variables in the dataset where associated with 
death within 28 days after admission, a logistic regression model was fit.
Step wise backward selection was used to exclude the variables, for which the fit coefficient
in the model did not significantly (alpha = 0.05) differ from zero.

To predict the length of stay in the ICU a linear regression and a random forest model where
fit. The data was split into a training and testing set. To find the respective variables to include, 
a lasso model was used on the training data. The accuracy of
the models was assessed, by making predictions for the testing data and comparing them to the true values.

## What I learned

- Using GitHub with R
- Examine missing values
- Exploratory data analysis using tidyverse
- Imputation of missing values using MICE
- Basic predictive modeling using caret
- Using lasso and random forest models

## Duration

- R: 45 h
- Other (writing etc.): 4 h

## Resources

Data Source: https://physionet.org/content/mimic2-iaccd/1.0/



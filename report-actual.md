# Module 12 Report Template

## Overview of the Analysis

In this analysis, I aimed to build a machine learning model to predict credit risk based on historical lending data. The data contains various financial details from which I needed to predict the 'loan_status' - whether a loan would likely be paid off on time or not. I processed the data, separating it into feature variables (`X`) and the target variable (`y`), and then I split this data into training and testing sets. I employed a logistic regression model, evaluated its performance, and attempted to improve it by using oversampling to address class imbalance.


## Results

Using bulleted lists, we summarize the balanced accuracy scores and the precision and recall scores of both machine learning models:

* Machine Learning Model 1 (Original Data):
  * Balanced Accuracy Score: 0.952
  * Precision:
    * Healthy Loan (0): 1.00
    * High-Risk Loan (1): 0.86
  * Recall:
    * Healthy Loan (0): 1.00
    * High-Risk Loan (1): 0.91

* Machine Learning Model 2 (Resampled Data):
  * Balanced Accuracy Score: 0.994
  * Precision:
    * Healthy Loan (0): 1.00
    * High-Risk Loan (1): 0.85
  * Recall:
    * Healthy Loan (0): 0.99
    * High-Risk Loan (1): 0.99

## Summary

The machine learning models performed with high accuracy, precision, and recall. Model 2, which was trained on resampled data, showed a slight improvement in balanced accuracy score and recall for high-risk loans compared to Model 1. Given the results, Model 2 is recommended for predicting credit risk, as it better identifies high-risk loans, which is critical for a financial institution looking to minimize defaults. The slight decrease in precision for high-risk loans in Model 2 is a trade-off for a significant increase in recall, meaning that while Model 2 might predict more false positives, it is better at catching the true positives, which is vital in credit risk assessment.

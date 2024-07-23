# Module 12 Report Template

## Overview of the Analysis

This analysis aimed to develop a machine-learning model to predict loan risk based on financial data.

The dataset contains financial attributes related to loan applicants, including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

The goal is to use this information to predict and classify loans into Healthy Loans (Class 0) and High-Risk Loans (Class 1) based on their associated risk factors or repayment potential.

The analysis began by collecting lending data from a CSV file, followed by dividing it into features and the target variable ('loan_status'). The data was split into training and testing sets for model training and evaluation.
  
The lending data provided included loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status. The goal was to predict if a loan is healthy or high-risk. The dataset contained loan information for 75036 healthy loans and 2500 high-risk loans. The dataset was first split into training and testing datasets to complete this analysis. 

After instantiating a logistic regression model from scikit-learn, the training data was fit to the model. Predictions of the test data were compared to the given labels. Due to the imbalanced nature of the given data, a resampled training dataset was created using RandomOverSampler from imbalanced-learn. A new logistic regression model was fit to the resampled data. Finally, the predictions of the resampled model were compared to the given results.

## Results

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
    * 
Accuracy: 94.4%

Precision:
Healthy Loans- 1.00
High-Risk Loans- .87

Recall:
Healthy Loans- 1.00
High-Risk Loans- .89
## Summary

The model performs well in predicting healthy loans. The logistic regression model predicts the 0(healthy loan) label correctly 100% of the time, but the 1 (high-risk loan) label with a precision of 87% and recall of 89%.



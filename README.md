# Credit Risk Report

## Overview of the Analysis


### The purpose of the analysis.

The purpose of the analysis is to build different logistic regression ML models, one trained with the original imbalanced data and one with random resampled data, and analyze how well the models will predict the creditworthiness of borrowers (either healthy or high risk of defaulting on their loans).

### Financial information the data was on, and what was needed to predict.

The financial information was about the loan (size and interest rate), income & debt (borrower's income and debt, debt-to-income ratio, # of accounts, derogatory marks), and also the loan status (healthy or risky). The loan status was used to compared the trained model's predictions using all the data except the loan status.

### Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

I was trying to predict if the loan status was more accurate based on the random oversampled data or the original imbalanced data.

### Describe the stages of the machine learning process you went through as part of this analysis.

Before training the model, I needed to separate the data I was using to train the model and the data that I was going to use to compare the predicted results from the model. After splitting the testing and training data, I instantiated the model, fit the data to the model, and made the predictions. Lastly, I printed the metrics so I could do the same process except with equal data points for both loan values using the random oversample module to balance out the data points.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * balanced accuracy score = 95.20%
    * 0 (Healthy Loans)   | precision = 100% | recall = 99% |
    * 1 (High-Risk Loans) | precision = 85% | recall = 91% |

* Machine Learning Model 2:
    * balanced accuracy score = 99.36%
    * 0 (Healthy Loans)   | precision = 100% | recall = 99% |
    * 1 (High-Risk Loans) | precision = 84% | recall = 99% |

## Summary

I think that the random oversampled data helped make better predictions than the original data across both classes as seen in the increase in the balanced accuracy score and recall for the high-risk loans. I think it is more important to predict the high-risk loans because high default rates can cause some issues for the lender if they get false predictions as opposed to false predictions for the healthy loans.

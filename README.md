# credit-risk-classification

# Module 20 Report

## Overview of the Analysis
This analysis aims to assess credit risk for a peer-to-peer lending company by predicting whether a loan is healthy (0) or high-risk (1) based on historical lending data.

## Purpose of the analysis
The purpose was to develop a machine learning model that can accurately classify loans as either healthy (likely to be repaid) or high-risk (likely to default), enabling the lending company to make more informed decisions about loan approvals.

## Financial information of the data

* Loan size: Amount of the loan (in dollars)

* Interest rate: Annual interest rate (%)

* Borrower income: Annual income of borrower (in dollars)

* Debt-to-income ratio: Ratio of borrower's debt to income

* Number of accounts: Number of credit accounts

* Derogatory marks: Negative marks on credit report

* Total debt: Borrower's total outstanding debt (in dollars)

* Target Variable (loan_status):
    * Binary classification label:

        * 0: Healthy loan (will be repaid) Count: 75,036 (96.8% of dataset)

        * 1: High-risk loan (likely to default) Count: 2,500 (3.2% of dataset)

## Stages of the machine learning process
1. Data Preparation:

    * Loaded and examined the data

    * Separated features (X) and target variable (y)

    * Split data into training and testing sets (75%/25%)

2. Model Training:

    * Initialized a Logistic Regression model

    * Trained the model on the training data

3. Model Evaluation:

    * Made predictions on the test set

    * Generated a confusion matrix

    * Calculated accuracy, precision, and recall scores

    * Created a classification report

## Methods used
The primary method used was Logistic Regression, which is good for binary classification problems. We chose this algorithm because:

    * It's interpretable and provides probability scores

    * Works well with numerical features

    * Efficient to train and predict

    * Provides good baseline performance

## Results

* Machine Learning Model 1: Logistic Regression

    * Accuracy: 0.99 (99% of predictions were correct)

    * Precision:

        * Class 0 (healthy): 1.00

        * Class 1 (high-risk): 0.87

    * Recall:

        * Class 0 (healthy): 1.00

        * Class 1 (high-risk): 0.94

## Summary

* The Logistic Regression model performed exceptionally well with 99% overall accuracy.

* The model performs perfectly at identifying Low Risk loans with 100% precision and recall.

* For High Risk loans, performance is slightly lower but still strong with 87% precision and 94% recall.

* In credit risk assessment, it's typically more important to correctly identify High Risk loans (class 1) to minimize defaults. The model's 94% recall for High Risk loans means it catches nearly all actual risky cases.

## Recommendantions

I strongly recommend using this Logistic Regression model because:

* Its overall accuracy is excellent (99%)

* It achieves near-perfect recall (94%) for the critical High Risk class

* The results are highly interpretable for business decisions

For potential improvements:

* Additional features might further improve High Risk loan detection

* Other models could be tested, but the current performance is already outstanding
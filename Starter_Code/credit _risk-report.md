# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to develop machine learning models to predict the creditworthiness of borrowers in a dataset of historical lending activity from a peer-to-peer lending services company. This is a classification problem with imbalanced classes, as healthy loans easily outnumber risky loans. The data was related to historical lending activity and includes information about borrowers and loans. The goal was to predict whether a loan is risky (class 1) or healthy (class 0).

## Stages of Machine Learning Process:
* Data Preprocessing: Data cleaning, feature engineering, and handling class imbalance.
* Model Selection: Logistic Regression is the chosen classifier.
* Model Training: Training models on the original dataset and a resampled dataset using RandomOverSampler.
* Model Evaluation: Calculating balanced accuracy, precision, and recall scores for both models.
* Generating a confusion matrix and classification report for model evaluation.

Logistic Regression is used for both models, and the RandomOverSampler technique is applied to resample the data to address class imbalance.

## Results

### Machine Learning Model 1:
* Balanced Accuracy Score: 0.95
* Precision (Class 0): 1.00
* Precision (Class 1): 0.85
* Recall (Class 0): 0.99
* Recall (Class 1): 0.91


### Machine Learning Model 2 (Resampled Data):
* Balanced Accuracy Score: 0.99
* Precision (Class 0): 1.00
* Precision (Class 1): 0.84
* Recall (Class 0): 0.99
* Recall (Class 1): 0.99


## Summary

The two logistic regression models were evaluated for their ability to predict creditworthiness, considering the imbalanced nature of the dataset. Model 2, which used resampled training data, outperformed Model 1 in terms of balanced accuracy, precision, and recall for class 1. The balanced accuracy increased from 0.95 to 0.99, indicating an improvement in model performance. In the context of credit risk prediction, it is crucial to identify risky loans (class 1) effectively. Model 2 performs better in this regard with higher precision and recall for class 1 compared to Model 1. Given the objective of identifying risky loans, Model 2 is recommended due to its superior performance. The choice of model may depend on the specific goals and priorities, but for credit risk assessment, Model 2 is preferred.

In summary, the logistic regression model with resampled training data (Model 2) is recommended for predicting creditworthiness in this imbalanced classification problem. It performs better in terms of balanced accuracy, precision, and recall, especially for class 1, which is of particular importance in credit risk assessment.

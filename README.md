# Module 12 Report Template

## Overview of the Analysis

In this analysis, the goal was to develop and evaluate machine learning models for credit risk classification using historical lending data. The analysis involved:

* Purpose: The primary purpose was to assess the creditworthiness of borrowers based on financial information.

* Data Description: The dataset contained features such as `loan_size`, `interest_rate`, `borrower_income`, `debt_to_income`, `num_of_accounts`, `derogatory_marks`, and `total_debt`. The target variable was `loan_status` (0 for healthy loans, 1 for high-risk loans).

* Variables of Interest: We focused on the balance of labels (healthy loans vs. high-risk loans) using `value_counts`.

* Machine Learning Process: The analysis proceeded through the following stages:
  - Data Preprocessing: Splitting data into training and testing sets.
  - Model Development: Building and training machine learning models, including Logistic Regression and Random Forest Classifier.
  - Model Evaluation: Assessing model performance in terms of balanced accuracy, precision, and recall.

## Results

Here are the results for the machine learning models:

* **Logistic Regression Model (Original Data):**
  - Balanced Accuracy Score: 0.952
  - Precision for Label 0 (Healthy Loans): 1.00
  - Recall for Label 0 (Healthy Loans): 0.99
  - Precision for Label 1 (High-Risk Loans): 0.85
  - Recall for Label 1 (High-Risk Loans): 0.91

* **Logistic Regression Model (Oversampled Data):**
  - Balanced Accuracy Score: 0.994
  - Precision for Label 0 (Healthy Loans): 1.00
  - Recall for Label 0 (Healthy Loans): 0.99
  - Precision for Label 1 (High-Risk Loans): 0.84
  - Recall for Label 1 (High-Risk Loans): 0.99

## Summary

Both models performed well, but the Logistic Regression Model with oversampled data outperformed the original model in terms of balanced accuracy, precision, and recall for high-risk loans. Given the importance of correctly identifying high-risk loans, we recommend deploying the Logistic Regression Model with oversampled data for credit risk assessment.

In summary, this model provides a highly reliable solution for assessing credit risk, achieving exceptional accuracy and balance in predicting both healthy and high-risk loans.

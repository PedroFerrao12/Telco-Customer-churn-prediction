# Telco-Customer-churn-prediction

# Customer Churn Prediction

## Project Overview
Customer churn prediction helps businesses identify customers likely to leave so they can take proactive retention actions.

This project builds a churn prediction model using the Telco Customer Churn dataset and AWS SageMaker Canvas.

## Objective
Predict whether a customer will churn and identify the key drivers influencing churn behavior.

## Dataset
Telco Customer Churn Dataset
- 9,292 customers
- 25 features
- Target variable: Churn (Yes/No)

## Feature Engineering
Created several engineered features including:

- AvgMonthlySpend
- TotalServices
- ContractRiskLevel
- CustomerValueScore
- TenureGroup

These features capture customer engagement and revenue potential.

## Model Performance

Accuracy: 83.37%  
F1 Score: 0.82  
AUC-ROC: 0.904

## Evaluation

Confusion Matrix:

TP: 712  
TN: 838  
FP: 195  
FN: 114

Recall: 86% of churners correctly identified.

## Business Insights

Key churn drivers:

- Month-to-month contracts
- Low tenure customers
- Higher monthly charges
- Customers with fewer services

## Business Impact

The model can identify high-risk customers and enable proactive retention strategies such as:

- targeted discounts
- service bundling
- loyalty incentives

## Tools Used

- AWS SageMaker Canvas
- PySpark
- Python
- Machine Learning

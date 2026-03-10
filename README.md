# Telco-Customer-churn-prediction

## Project Overview

Customer churn is a major challenge for subscription-based businesses because losing customers directly reduces recurring revenue. Predicting churn enables companies to identify at-risk customers early and take proactive retention actions.

This project analyzes telecom customer behavior and builds a predictive model to identify customers likely to churn. The model was developed using Amazon SageMaker Canvas and enhanced with feature engineering to capture customer engagement and revenue value.

The goal of this project is not only to predict churn but also to extract actionable business insights that can help improve customer retention strategies.

---

## Dataset

The dataset used in this project is the Telco Customer Churn dataset containing customer demographics, service subscriptions, and billing information.

**Dataset characteristics**

* ~9,000 customers
* 25 features
* Target variable: **Churn (Yes/No)**

Example features include:

* tenure (customer lifetime)
* MonthlyCharges
* TotalCharges
* Contract type
* Internet services
* Payment method

---

## Project Workflow

The project follows a typical data science pipeline:

1. Data Exploration (EDA)
2. Data Cleaning
3. Feature Engineering
4. Model Training using Amazon SageMaker Canvas
5. Model Evaluation
6. Business Insight Extraction

---

## Model Development

The predictive model was built using **Amazon SageMaker Canvas**, which automatically evaluates multiple machine learning algorithms and selects the best-performing model.

To address class imbalance between churners and non-churners, SMOTE oversampling was applied during training.

---

## Model Performance and Evaluation

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 83.37% |
| Precision | 78.5%  |
| Recall    | 86.2%  |
| F1 Score  | 0.82   |
| AUC-ROC   | 0.904  |


| Actual Stay  | 195             | 838            |

Interpretation:

* 712 churners were correctly identified.
* 114 churners were missed by the model.
* 195 customers were incorrectly flagged as churners.

This tradeoff favors higher recall, which is often desirable in churn prediction because missing a churner can lead to revenue loss.

---

## Business Recommendations

Based on the findings, several strategies could help reduce churn:

* Encourage longer-term contracts through discounts or incentives.
* Improve onboarding experiences for new customers.
* Promote service bundles to increase customer engagement.
* Deploy the churn model to identify high-risk customers and trigger retention campaigns.

---

## Tools & Technologies

* Python PySpark
* Amazon SageMaker Canvas
* Pandas
* Matplotlib

---

## Author
Pedro Ferrao Junior
  

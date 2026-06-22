Customer Churn Prediction Using Machine Learning
Project Overview

Customer churn is a major challenge for telecommunication companies. Acquiring new customers is often more expensive than retaining existing ones. This project aims to predict whether a customer is likely to leave a telecom service provider using machine learning techniques.

The project analyzes customer demographics, subscription details, billing information, and service usage patterns to identify factors influencing churn.

Problem Statement

The objective of this project is to:

Predict customer churn using machine learning.
Identify the key factors contributing to customer churn.
Provide business insights to improve customer retention strategies.
Dataset

Dataset: Telco Customer Churn Dataset

Total Records: 7043
Features: 21 original features
Target Variable: Churn

Key features include:

Gender
Senior Citizen
Tenure
Internet Service
Contract Type
Payment Method
Monthly Charges
Total Charges


Project Workflow
Raw Data
    ↓
Data Cleaning
    ↓
Exploratory Data Analysis (EDA)
    ↓
Preprocessing & Feature Engineering
    ↓
Train-Test Split
    ↓
Model Training
    ↓
Model Evaluation
    ↓
SHAP Explainability
    ↓
Business Insights
Data Preprocessing

The following preprocessing steps were performed:

Removed unnecessary columns
Handled missing values
Converted categorical variables into numerical format using One-Hot Encoding
Created feature matrix (X) and target variable (y)
Split data into training and testing sets (80:20)
Models Used
1. Logistic Regression

Selected as the final model due to its superior overall performance.

2. Random Forest Classifier

Used to compare performance with an ensemble-based approach.

3. XGBoost Classifier

Used as an advanced boosting algorithm for performance comparison.

Model Evaluation Metrics

The following evaluation metrics were used:

Accuracy
Precision
Recall
F1 Score
ROC-AUC Score
Confusion Matrix
Results
Model	Accuracy	ROC-AUC
Logistic Regression	0.80	0.8426
Random Forest	0.79	~0.81
XGBoost	~0.78	0.8186
Final Selected Model

Logistic Regression

Reasons:

Highest ROC-AUC score
Best balance between Precision and Recall
Better churn detection performance compared to Random Forest and XGBoost
SHAP Explainability

SHAP (SHapley Additive exPlanations) was used to interpret model predictions.

Important features identified:

Tenure
Total Charges
Contract Type
Internet Service (Fiber Optic)
Paperless Billing
Payment Method (Electronic Check)

Key findings:

Customers with lower tenure are more likely to churn.
Customers with two-year contracts are less likely to churn.
Fiber Optic users showed higher churn probability.
Electronic Check payment method is associated with higher churn risk.
Business Insights

Based on the analysis:

Focus retention campaigns on new customers.
Encourage customers to move to long-term contracts.
Improve customer experience for Fiber Optic users.
Monitor customers using Electronic Check payments.
Offer loyalty benefits to customers with low tenure.
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
XGBoost
SHAP
Jupyter Notebook
Git & GitHub
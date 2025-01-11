# Credit Card Transactions Fraud Detection Project
This repository hosts a machine learning project aimed at detecting fraudulent credit card transactions using the dataset available on Kaggle: [Credit Card Transactions Dataset](https://www.kaggle.com/datasets/priyamchoksi/credit-card-transactions-dataset/code). The project explores data preprocessing, feature engineering, and implementing machine learning models to classify transactions as fraud or non-fraud effectively.

## Table of Contents
* Dataset Overview
* Project Objectives
* Features and Description
* Project Workflow
* Modeling Techniques
* Future Work

## Dataset Overview
The dataset is sourced from Kaggle and contains anonymized credit card transactions labeled as fraudulent or non-fraudulent.
* Dataset Size: 300 MB
* Records: Over 250,000 transactions
* Fraud Label: Binary (1 = Fraudulent, 0 = Non-fraudulent)
Ensure you download the dataset and place it in the appropriate directory before running the code.

## Project Objectives
* Understand the characteristics of fraudulent transactions through exploratory data analysis (EDA).
* Build and optimize machine learning models to detect fraud effectively.
* Evaluate the performance of models using metrics like precision, recall, F1-score, and AUC-ROC.

## Features and Description

| Feature Name | 	Description |
|-----------------------|--------------------------------------------|
| trans_date_trans_time	| Timestamp of the transaction. |
| card_num	| Unique identifier for each credit card. |
| merchant	| Merchant where the transaction occurred. |
| amt	| Transaction amount. |
| gender	| Gender of the cardholder. |
| city	| City where the transaction occurred. |
| state	| State where the transaction occurred. |
| zip	| ZIP code of the transaction location. |
| lat and long	| Latitude and longitude of the transaction location. |
| is_fraud	| Target variable indicating whether the transaction was fraudulent (1) or not (0). |

## Project Workflow
### Data Preprocessing:
* Handle missing values.
* Drop the extra index row.

### Exploratory Data Analysis (EDA):
* Analyze patterns in fraudulent transactions.

### Feature Engineering:
* Dropp irrevant rows.
* Encode categorical variables.
* Create new features from existing data (e.g., Hour).
* Handle class imbalance using undersampling.
* Normalize numerical features.

### Model Building:
* Train machine learning models, including Logistic Regression, Random Forest, SVC, and Gradient Boosting.
* Fine-tune hyperparameters for optimal performance.

### Evaluation:
* Use precision, recall, F1-score, and AUC-ROC to evaluate model performance.

### Deployment:
Implement a real-time fraud detection system using Flask or Streamlit.

## Modeling Techniques
This project leverages the following machine learning models:
* Logistic Regression: A baseline model for binary classification.
* Support Vector Machine: To compare with LR.
* Random Forest: A robust model for handling complex datasets.
* Gradient Boosting (XGBoost/LightGBM): For handling class imbalance and achieving high accuracy.

# Future Work
* Implement real-time fraud detection using an API.
* Incorporate unsupervised learning techniques to detect novel fraud patterns.
* Experiment with explainable AI tools like SHAP to interpret model predictions.

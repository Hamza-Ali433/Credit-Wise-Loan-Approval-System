# CreditWise Loan Approval Predictor

## Overview

CreditWise Loan Approval Predictor is an end-to-end Machine Learning classification project that predicts whether a loan application should be approved or rejected based on an applicant's financial, demographic, and credit-related information.

The project simulates a real-world banking scenario where financial institutions need to process hundreds of loan applications efficiently while minimizing risk. By leveraging Machine Learning, the system helps identify trustworthy applicants and supports faster, more consistent, and data-driven decision-making.

---

## Problem Statement

Traditional loan approval processes rely heavily on manual verification of applicant information such as income, employment status, credit score, loan amount, and existing liabilities. This process can be time-consuming, inconsistent, and prone to human error.

The objective of this project is to build a Machine Learning system capable of predicting loan approval outcomes using historical loan application data.

---

## Dataset Features

The dataset contains information about loan applicants, including:

* Applicant Income
* Coapplicant Income
* Employment Status
* Age
* Marital Status
* Dependents
* Credit Score
* Existing Loans
* Savings
* Collateral Value
* Loan Amount
* Loan Tenure
* Education Level
* Loan Purpose
* Property Area
* Gender
* Employer Category

### Target Variable

* Loan Approved (0 = Rejected, 1 = Approved)

---

## Project Workflow

### 1. Data Preprocessing

* Loaded dataset using Pandas
* Checked data types and missing values
* Removed inconsistencies and prepared data for analysis

### 2. Missing Value Handling

* Numerical columns filled using Mean Imputation
* Categorical columns filled using Most Frequent Imputation

### 3. Exploratory Data Analysis (EDA)

Performed data visualization and statistical analysis to understand patterns and relationships within the dataset.

Visualizations include:

* Loan Approval Distribution
* Correlation Heatmap
* Income Distribution
* Feature Relationships
* Category-wise Approval Analysis

### 4. Feature Engineering

Created additional features to improve model performance:

* DTI_Ratio_sq
* Credit_Score_sq

### 5. Feature Encoding

Applied:

* One-Hot Encoding
* Drop First Category to avoid Dummy Variable Trap

### 6. Feature Scaling

Applied StandardScaler to normalize feature values before model training.

---

## Machine Learning Models

The following classification algorithms were implemented and compared:

### Logistic Regression

A baseline classification model used for binary prediction tasks.

### K-Nearest Neighbors (KNN)

A distance-based algorithm that classifies applicants based on the nearest training examples.

### Gaussian Naive Bayes

A probabilistic classifier based on Bayes' Theorem.

---

## Model Evaluation

The models were evaluated using:

* Accuracy Score
* Precision Score
* Recall Score
* F1 Score
* Confusion Matrix
* Classification Report

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

## Project Structure

```text
CreditWise-Loan-Approval-Predictor/

│
├── Loan_Approval_Project.ipynb
├── loan_approval_data.csv
├── README.md
│
├── plots/
│   ├── loan_approval_distribution.png
│   ├── correlation_heatmap.png
│   ├── income_analysis.png
│   └── approval_analysis.png
│
└── requirements.txt
```

---

## Key Learning Outcomes

Through this project, I gained hands-on experience in:

* Data Cleaning and Preprocessing
* Missing Value Handling
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Feature Encoding
* Feature Scaling
* Classification Algorithms
* Model Evaluation
* Building End-to-End Machine Learning Pipelines

---

## Future Improvements

* Hyperparameter Tuning using GridSearchCV
* Random Forest Classifier
* XGBoost Classifier
* Cross Validation
* Model Deployment using Streamlit or Flask
* Feature Selection Techniques

---




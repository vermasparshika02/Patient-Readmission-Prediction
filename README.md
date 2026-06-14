# Patient-Readmission-Prediction
Overview

This project develops machine learning models to predict whether a patient will be readmitted within 30 days of hospital discharge. Early identification of high-risk patients can help healthcare providers improve discharge planning, optimize resource allocation, and reduce preventable readmissions.

Dataset

The project uses an Indian hospital admissions dataset containing patient demographics, clinical measurements, hospital information, and admission details. Key features include:

Length of Stay (LOS)
Charlson Comorbidity Index
HbA1c
Creatinine
Haemoglobin
Systolic Blood Pressure
Discharge Type
Number of Procedures
Hospital Information

The target variable is:

readmitted_30d (1 = Readmitted within 30 days, 0 = Not Readmitted)
Objectives
Perform data cleaning and preprocessing
Analyze class imbalance and patient readmission patterns
Build baseline machine learning models for readmission prediction
Compare model performance using healthcare-relevant metrics
Identify the most important factors influencing readmission risk
Methodology
Data Cleaning and Missing Value Handling
Exploratory Data Analysis (EDA)
Feature Encoding and Preprocessing
Train-Test Split with Stratified Sampling
Logistic Regression Model
Random Forest Model
Performance Evaluation using:
Accuracy
Precision
Recall
ROC-AUC
Feature Importance Analysis
Results
Logistic Regression achieved a ROC-AUC of approximately 0.74
The dataset exhibited class imbalance, making Recall a critical evaluation metric
Logistic Regression outperformed Random Forest in identifying high-risk patients, making it more suitable for healthcare screening applications
Key Insights

Feature importance analysis identified the following predictors as major contributors to readmission risk:

Haemoglobin
Length of Stay (LOS)
Creatinine
Systolic Blood Pressure
Charlson Comorbidity Index
HbA1c

These findings suggest that disease severity, comorbidity burden, and abnormal laboratory values play a significant role in patient readmissions.

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Joblib
Project Structure
├── admissions.csv
├── notebooks/
│   └── Patient_Readmission_Prediction.ipynb
├── models/
│   └── patient_readmission_model.pkl
├── images/
│   ├── roc_curve.png
│   └── feature_importance.png
└── README.md
Future Improvements-
Hyperparameter tuning using GridSearchCV
Handling class imbalance with SMOTE
XGBoost and LightGBM implementation
Deployment using Flask or Streamlit
Explainable AI using SHAP values

# Patient Readmission Prediction

A machine learning project focused on predicting 30-day hospital readmission risk using Indian healthcare admission data. The workflow includes data cleaning, exploratory data analysis (EDA), feature engineering, class imbalance assessment, and predictive modeling.

Two baseline models—Logistic Regression and Random Forest—were developed and evaluated using ROC-AUC, recall, precision, and accuracy. Logistic Regression achieved superior recall, making it more effective for identifying high-risk patients in an imbalanced healthcare setting.

Feature importance analysis highlighted clinical indicators such as haemoglobin, creatinine, length of stay, HbA1c, systolic blood pressure, and comorbidity burden as key predictors of readmission risk.

## Tech Stack
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Key Outcomes
- Built end-to-end readmission prediction pipeline
- Achieved ROC-AUC ≈ 0.74
- Compared Logistic Regression and Random Forest models
- Identified major factors influencing patient readmission
- Generated actionable healthcare insights through model interpretation

# Home Credit Default Risk Prediction

## Project Overview
This project uses machine learning to predict whether loan applicants may experience payment difficulties. The goal is to identify potential default risk using applicant and financial information.

## Problem Statement
Financial institutions need to assess the risk of applicants experiencing difficulties in repaying loans. This project explores applicant data and builds machine learning models to predict payment difficulties.

## Objectives
- Perform exploratory data analysis (EDA).
- Clean and preprocess the dataset.
- Perform feature engineering.
- Build and compare machine learning models.
- Tune the XGBoost model.
- Interpret model predictions using SHAP.

## Dataset
The project uses the Home Credit Default Risk dataset.

- Training records: 307,511 applicants.
- Original features: 122 columns.
- Target variable: `TARGET`.
  - `0`: No payment difficulties.
  - `1`: Payment difficulties.

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- XGBoost
- SHAP
- Jupyter Notebook

## Machine Learning Models
The following models were developed and evaluated:
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

XGBoost was further improved using RandomizedSearchCV for hyperparameter tuning.

## Final Model Performance

| Metric | Score |
|---|---:|
| Accuracy | 70.65% |
| Precision | 17.03% |
| Recall | 68.08% |
| F1-score | 27.25% |
| ROC-AUC | 76.05% |
| PR-AUC | 25.24% |

## Model Interpretation
SHAP analysis was used to identify influential features. EXT_SOURCE_1, employment duration, age, education and annuity amount were among the most influential features.

## Conclusion
The final XGBoost model identifies a substantial proportion of applicants who experience payment difficulties. However, its low precision indicates that many high-risk predictions are incorrect. Therefore, the model can support risk assessment but should not be used as the sole basis for lending decisions.


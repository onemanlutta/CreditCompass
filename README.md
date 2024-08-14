# Loan Approval Prediction Project

## Project Overview

This project aims to develop a machine learning model to predict loan approval based on various applicant attributes. By analyzing temporal trends, demographic and economic patterns, income ratios, and geographical differences, the project seeks to enhance the fairness and efficiency of lending decisions.

### Objective
To create a machine learning model that predicts loan approval based on various applicant attributes.

## Data Sources
- **Primary Data**: Kaggle Lending Club Data
- **Geographical Data**: `us-states.json` file

## Tools and Technologies
- **Development Environment**: Jupyter Notebook, VS Code
- **Languages and Libraries**: Python, Pandas, Matplotlib, Seaborn, Plotly, XGBoost, scikit-learn
- **Data Handling**: JSON, CSV, PostgreSQL
- **Web Framework**: Flask
- **Visualization**: Leaflet, D3.js

## Data Preparation
- **Data Cleaning**: Removal of missing or irrelevant data.
- **Normalization & Standardization**: Scaling features to ensure uniformity.
- **Feature Engineering**: Identification and creation of critical features.

## Model Performance
- **Logistic Regression**: Accuracy = 0.5994
- **Decision Tree**: Accuracy = 0.6527
- **Random Forest**: Accuracy = 0.6883
- **Gradient Boosting**: Accuracy = 0.6816
- **XGBoost**: Accuracy = 0.7296 (Best Model)
  - **ROC AUC**: 0.81

### Feature Importance
1. `int_rate`: 0.158708
2. `dti`: 0.135081
3. `income_to_loan_ratio`: 0.118495
4. `installment`: 0.117501
5. `annual_inc`: 0.101025
6. `addr_state`: 0.088280
7. `loan_amnt`: 0.072905
8. `emp_length`: 0.052212
9. `purpose`: 0.031595
10. `mort_acc`: 0.028045
11. `term`: 0.027703
12. `delinq_2yrs`: 0.021732
13. `grade`: 0.016636
14. `home_ownership`: 0.015951
15. `pub_rec`: 0.014133

## Key Results
- **Best Models**: XGBoost and Random Forest exhibited the highest accuracy and ROC AUC scores, effectively capturing patterns in loan approval data.
- **Significant Predictors**:
  - Interest rate, debt-to-income ratio, income-to-loan ratio, installment capability, and annual income.
  - Geographical trends and employment length also impacted loan approval.
  - Home ownership status showed relevance in loan approval likelihood.
- **Model Insights**: Ensemble methods (Random Forest, XGBoost) were effective for handling complex datasets. Models with fewer features performed worse compared to those with more comprehensive feature sets.

## GitHub Documentation
- **Repository**: [Link to Repository](https://github.com/your-repo-link)
  - Free of unnecessary files and folders.
  - Includes a `.gitignore` file to exclude irrelevant files.
- **README**: Provides a polished presentation of the project's content and setup.

## Group Members
- Rudi Espinoza
- Maero Lutta
- Pablo Guinda
- Diana Tarasovers
- Eunice Mwangi

## Flask App Setup

### Steps to Set Up and Run the Flask App
1. **Install Dependencies**:
   ```bash
   pip install flask pandas numpy scikit-learn xgboost matplotlib seaborn plotly
   

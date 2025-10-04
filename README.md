# Credit Score Prediction using Logistic Regression

This project focuses on predicting a borrower's credit score category using a Logistic Regression model built with Python.
It demonstrates a complete data science workflow including data preprocessing, feature engineering, scaling, model training, evaluation, and deployment.

---

## Project Overview

The Credit Score model predicts whether a borrower falls into a certain credit score category (e.g., good, average, poor) based on financial and demographic features.
Accurate prediction helps financial institutions manage risk and make better lending decisions.

---

## Workflow Summary

This notebook includes the main steps of a credit risk modeling process:

1. Library Imports
- Imported necessary Python libraries for data manipulation, modeling, and evaluation.

2. Exploratory Data Analysis (EDA)
- Used `describe()` to summarize the dataset.
- Checked for missing values (`isnull()`) and data types.
- Conducted univariate analysis to examine each feature individually.
- Visualized distributions and class balance.

3. WOE and Normality Checks
- Applied Weight of Evidence (WOE) transformation for categorical variables where needed.
- Tested normality of continuous variables using the Kolmogorov–Smirnov test.

4. Correlation Analysis
- Analyzed correlation and intercorrelation between predictors to understand relationships and check for potential multicollinearity.
- No new features were created from this analysis.

5. Input-Output Preparation
- Defined the predictor variables (X) and the target variable (y).

6. Model Training
- Split data into training and testing sets.
- Trained the Logistic Regression model:
  ```python
  from sklearn.linear_model import LogisticRegression

7.Model Evaluation

- Evaluated model performance using metrics such as Gini coefficient, ROC-AUC score, precision, recall, and precision-recall curve.
- Analyzed results to understand model strengths and weaknesses.
- Evaluated the model on training and test sets using fit and evaluate.

8.Deployment
The trained Logistic Regression model is ready to generate credit score predictions on new data.



  
  model = LogisticRegression()
  model.fit(X_train, y_train)

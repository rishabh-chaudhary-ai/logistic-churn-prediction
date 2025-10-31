# Customer Churn Prediction and Analysis
## Project Overview

Customer churn is a phenomenon when customers stop using a company's services/products which can negatively impact revenue and growth. Predicting which customers are likely to churn enables proactive retention strategies, reducing loss and enhancing business sustainability.
This project aims to build an end-to-end machine learning solution to accurately predict customer churn based on telecom customer data. It integrates data preprocessing, feature engineering, multiple model training and evalutaion steps, hyperparameter tuning, and model explainability techniques.

## Problem Statement
Telecom companies face fierce competition and costly customer attrition. Identifying churners early allows targeted interventions such as customized offer or improved service. The challenge lies in effectively analyzing complex customer data and building robust predictive models that generalize well.

## Solution Approach

The approach consists of the following key steps:

### Data Exploration and Preprocessing:
- Import and explore the telecom churn dataset, examining data types, distributions and missing values.
- Handle missing values by appropriate imputation and transform categorical variables into machine-readable formats.
- Remove irrelevant or highly correlated features that do not contribute to model accuracy.
- Normalize numerical features using feature scaling for consistent model input.

### Feature Engineering:
- Encode categorical variables using label encoding for binary classes and one-hot encoding for multi-class.
- Split data into training and test sets with stratification to preserve class distribution.
- Address class imbalance, common in churn datasets using synthetic minority oversampling technique (SMOTE).

### Model Building and Hyperparameter tuning:
- Train several machine learning classifiers including Logistic Regression, Suport Vector Machines, Decision Trees, Random Forests, and gradient boosting methods (XGBoost, LightGBM, CatBoost)
- Optimize model performance using grid search hyperparameter tuning with cross-validation.
- Incorporate class weight adjustments alongside SMOTE to further mitigate imbalance effects.

### Model Evaluation:
- Evaluate models on test data using accuracy, f1-score, precision, recall and classification reports.
- Select the best performing model based on balanced metrics and generalization capability.

### Explainability:
- Use SHAP (Shapely additive exPlanations) values on the final model to interpret feature importance.
- Provide insights at both global and individual prediction levels for business stakeholders.

## Results

The tuned ensemble models, particularly Random Forest and Gradient Boosting (XGBoost and LightGBM), achieved around 86% accuracy on unseen test data, demonstrating strong predictive power, SHAP-based explainability highlighted key churn drivers such as contract type, monthly charges, tenure, and payment method.

## Conclusion

This project presents a practical and scalable machine learning solution to customer churn prediction in telecom. It combines robust data preprocessing, state-of-the-art models, and interpretability to enable actionable business decisions. This end-to-end pipeline can be adapted to similar customer retention challenges across industries.

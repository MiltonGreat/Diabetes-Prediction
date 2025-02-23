# Diabetes Prediction

## Overview 

This project aims to predict the likelihood of diabetes in individuals based on various health-related features. Using machine learning techniques, the goal is to build a model that classifies individuals as either diabetic or non-diabetic, based on their age, BMI, glucose levels, insulin levels, skin thickness, and other health indicators.

### Dataset

The dataset used for this project contains information on various health metrics for patients, including the following features:

- **Age**: Age of the individual
- **BMI**: Body Mass Index
- **Glucose**: Glucose concentration in the blood
- **Insulin**: Insulin level in the blood
- **SkinThickness**: Skin thickness measurement (for body fat analysis)
- **DiabetesPedigreeFunction (DPF)**: A function that helps predict diabetes based on family history
- **Outcome**: Whether the individual is diabetic (1) or non-diabetic (0)

### Methodology

1. **Data Exploration**: We start by analyzing the dataset for missing values, feature distributions, and potential outliers. Visualizations such as histograms, box plots, and violin plots are used to understand the relationships between features and the target variable (Outcome).

2. **Data Preprocessing**: Missing values are handled, categorical features are encoded, and features are normalized or scaled as needed. The data is then split into training and test sets.

3. **Modeling**: Several classification models are trained, including Logistic Regression and Random Forest. Hyperparameter tuning and cross-validation are applied to improve performance.

4. **Model Evaluation**: The models are evaluated using metrics such as accuracy, precision, recall, and F1-score. A confusion matrix is generated to visualize the model's classification performance. Due to class imbalance, we focus on precision and recall rather than accuracy alone.

### Results

- The model achieved an accuracy of 77.92%, with strong performance for non-diabetic cases (class 0) but weaker performance for diabetic cases (class 1).
- Glucose, BMI, and Insulin levels were identified as key features influencing the likelihood of diabetes.
- The R² score was low, indicating the model did not capture the underlying patterns in the data well and further improvements are needed.

### Future Work

The model provides useful insights into predicting diabetes, but there is significant room for improvement. Future work could focus on:

1. Improving model accuracy by tuning hyperparameters.
2. Implementing techniques to handle class imbalance (e.g., oversampling).
3. Exploring advanced models (e.g., XGBoost, neural networks).
4. Conducting a fairness analysis to ensure no demographic bias in predictions.

### Source

https://www.kaggle.com/datasets/mathchi/diabetes-data-set

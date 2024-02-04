# Diabetes Prediction Model

This repository contains a Jupyter Notebook (`DM_Project_9731084.ipynb`) that focuses on building a diabetes prediction model using XGBoost, a popular machine learning algorithm. The notebook walks through the various steps involved in data preprocessing, model creation, parameter tuning, and evaluation.

## Table of Contents
1. [Introduction](#introduction)
2. [Preprocessing](#preprocessing)
   - [Handling Missing Data](#handling-missing-data)
   - [Renaming Columns](#renaming-columns)
   - [Normalization](#normalization)
   - [One-Hot Encoding](#one-hot-encoding)
3. [Model Building](#model-building)
   - [Train-Test Split](#train-test-split)
   - [XGBoost Classifier](#xgboost-classifier)
   - [Model Evaluation](#model-evaluation)
4. [Hyperparameter Tuning](#hyperparameter-tuning)
5. [Conclusion](#conclusion)

## Introduction <a name="introduction"></a>
The primary objective of this project is to predict diabetes using a machine learning model. The dataset (`diabetes.csv`) is preprocessed and utilized to train an XGBoost classifier. The model's performance is evaluated, and hyperparameter tuning is performed to enhance its predictive capabilities.

## Preprocessing <a name="preprocessing"></a>
### Handling Missing Data <a name="handling-missing-data"></a>
The notebook addresses missing data by identifying and replacing null values with the mode or relevant statistical measures. Rows with unknown values are removed to ensure data integrity.

### Renaming Columns <a name="renaming-columns"></a>
Column names are checked for spaces and replaced with underscores to facilitate ease of use in subsequent analyses.

### Normalization <a name="normalization"></a>
Three specific columns are normalized: BMI is binned into categories, and two health columns are normalized using min-max scaling.

### One-Hot Encoding <a name="one-hot-encoding"></a>
Categorical features are one-hot encoded to convert them into a format suitable for machine learning algorithms.

## Model Building <a name="model-building"></a>
### Train-Test Split <a name="train-test-split"></a>
The dataset is split into training and testing sets to enable the model to learn from one subset and validate its performance on another.

### XGBoost Classifier <a name="xgboost-classifier"></a>
An XGBoost classifier is employed for diabetes prediction, and the model is trained on the training set.

### Model Evaluation <a name="model-evaluation"></a>
The model's accuracy, recall, and precision are evaluated on both the training and testing sets. Confusion matrices are generated to visualize the model's performance.

## Hyperparameter Tuning <a name="hyperparameter-tuning"></a>
The notebook explores hyperparameter tuning using a grid search approach to optimize the XGBoost model's performance. The best parameters are identified, and the model is retrained with these parameters.

## Conclusion <a name="conclusion"></a>
According to the drawn charts, the only parameter that has a more significant impact is the learning rate; the other parameters, as observed, have horizontal plots, indicating that they do not have much influence on the model's performance.

Feel free to explore the notebook for a detailed walkthrough of each step and the corresponding code.

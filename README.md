# Credit Card Default Analysis

## Overview

This GitHub repository contains the code and documentation for a comprehensive analysis of credit card default prediction. The project encompasses various stages of data analysis, preprocessing, feature selection, modeling, and evaluation. Three machine learning models, namely Logistic Regression, Random Forest, and Neural Network, are employed to predict credit card default, with a focus on addressing class imbalance and optimizing model performance.

## Introduction

Credit card default prediction is a critical task for financial institutions to manage risk effectively. This project aims to develop predictive models that can identify customers who are likely to default on their credit card payments.

## Dataset

The dataset is obtained from https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset, and contains information about credit card holders, including demographic features and credit history. The target variable is whether a customer defaults on their credit card payment or not.

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis is performed to gain insights into the dataset, understand the distributions of variables, and identify any patterns or anomalies that may exist in the data.

## Data Preprocessing

Data preprocessing involves standardizing labels, creating dummy variables for categorical features, dropping irrelevant columns, and removing outliers to prepare the data for modeling.

## Feature Selection

Feature selection employs the chi-squared test to determine whether there is a relationship between two categorical variables, and if so, whether that relationship is statistically significant. Subsequently, the results from the chi-squared test are combined with all numerical variables, and logistic regression is performed. Following this logistic regression step, feature importance is calculated to select the most relevant features for the modeling phase.

## Model Building

Three machine learning models are built: Logistic Regression, Random Forest, and Neural Network. These models are trained on the preprocessed data to predict credit card default.

## Hyperparameter Tuning

Grid search is used to optimize the hyperparameters of the models.

## Class Imbalance Handling

Class imbalance is addressed using Synthetic Minority Over-sampling Technique (SMOTE) to balance the dataset and improve model performance on minority class prediction.

## Model Evaluation

Model performance is evaluated using the F1-score, a metric that balances precision and recall. The F1-score provides a comprehensive view of model effectiveness in predicting credit card defaults. Random Forest gives the highest F-1 score of 0.7871.


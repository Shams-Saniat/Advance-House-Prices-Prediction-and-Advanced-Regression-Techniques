# House Price Prediction - Advanced Regression Techniques

## Overview

**Project of the course CSE445 (Machine Learning)**  
This project aims to predict the sales prices of houses, a common problem for potential homebuyers, especially those unfamiliar with the area. By leveraging advanced regression techniques, the project provides users with a reliable estimate of house prices, helping them avoid overpaying due to unscrupulous sellers.

This project specifically addresses a Kaggle competition problem, where the objective is to predict the sales price (`SalePrice`) for each house in the test set.

## Project Description

### Problem Statement
House prices can be highly unpredictable, often leading to confusion among buyers. This project seeks to solve this problem by predicting house prices based on various features, helping users make informed purchasing decisions.

### Project Objectives
- Predict the sales price for each house.
- For each `Id` in the test set, predict the value of the `SalePrice` variable.

## How We Solved It

### 1. Data Analysis
- **Missing Values:** Identification and handling of missing data.
- **Numerical Variables:** Analysis of distribution.
- **Categorical Variables:** Examination of cardinality and relationships.
- **Outliers:** Detection and treatment of outliers.
- **Variable Relationships:** Studied the relationship between independent and dependent variables.

### 2. Feature Engineering
- Handled missing values.
- Managed temporal variables.
- Processed categorical variables by removing rare labels.
- Standardized the values of variables to ensure consistency.

### 3. Feature Selection
- Used variance threshold and correlation tests to select features.
- Experimented with dropping irrelevant features, but this approach did not reduce errors in Kaggle submissions.

### 4. Model Building
- Utilized a train-test split with 66% of the data for training and 33% for testing.
- Initially used linear models, with **Ridge Regression** performing best.
- Eventually, **Random Forest Regression** outperformed all other models due to the non-linear relationships in the dataset.

## Results

### Model Performance on Training Set
- **Linear Regression:** 0.824
- **Ridge Regression:** 0.842
- **Lasso Regression:** 0.846
- **SVR Regression:** -0.0157
- **Random Forest Regression:** 0.981

### Kaggle Test Data
- The Random Forest model provided the best performance with a significant improvement in prediction accuracy.

## Repository Structure

- **data/**: Contains training and test datasets.
- **notebooks/**: Jupyter notebooks used for data analysis, feature engineering, and model training.
- **models/**: Saved models for further use or evaluation.
- **results/**: Output predictions and performance metrics.
- **README.md**: Project overview and instructions.

## Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Required Python packages: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Shams-Saniat/Advance-House-Prices-Prediction-and-Advanced-Regression-Techniques.git

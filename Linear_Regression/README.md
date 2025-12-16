# Linear Regression

## Overview
This project applies Linear Regression from scratch using Gradient Descent to predict a continuous numerical value from a structured tabular dataset. The goal is to understand how regression models learn relationships between features and a target variable.

## Dataset
**Target variable:** Car price (continuous value, e.g., in lakhs)  
**Input features:** Year of manufacture, kilometers driven, mileage, engine capacity, power, number of seats, along with other vehicle attributes

## Problem Statement
To build a Linear Regression model that can accurately predict the target variable based on the given input features and evaluate its performance using regression metrics.

## Approach
- Loaded the Train.csv and Test.csv car price datasets and inspected columns like Year, KilometersDriven, Mileage, Engine, Power, Seats, and Price.
- Preprocessed the data by extracting numeric values from string features with units (e.g., "23.84 kmpl", "1199 CC", "84 bhp") and dropping rows with missing values.
- Applied mean normalization / standardization to selected numeric features to help gradient descent converge more smoothly.
- Implemented a Linear Regression model from scratch using NumPy (manual weights, bias, and gradient descent) instead of using scikit-learn.
- Tracked the cost (MSE) across iterations and evaluated the trained model on the test set using metrics like MSE, RMSE, and R² score.

## Key Concepts Explored
- Linear relationship between car features (year, usage, mileage, engine size, power, seats) and target price.
- Definition and implementation of the cost function (Mean Squared Error) and how gradient descent minimizes this error by updating weights and bias.
- Importance of feature scaling (mean normalization/standardization) for stable and faster gradient descent.
- Basic regression evaluation: interpreting RMSE and R² score to understand how well the model predicts unseen car prices.
- Underfitting & Ovrfitting and limitations of linear models

## Tools & Libraries
- Python  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib  



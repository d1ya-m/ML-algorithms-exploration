# Linear Regression

## Overview
This project implements **Linear Regression from scratch using Gradient Descent** to predict **used car prices** from a structured tabular dataset. The objective is to understand how regression models learn relationships between input features and a continuous target variable.

---

## Project Structure
```
.
├── Train.csv
├── Test.csv
├── task2_0_linearregression.ipynb
└── README.md
```

---

## Dataset
The dataset consists of used-car listings with numerical and categorical attributes.

**Target variable:** Car price (continuous value, e.g., in lakhs)
**Input features:** Year of manufacture, kilometers driven, mileage, engine capacity, power, number of seats, along with other vehicle attributes

---

## Problem Statement
To build a Linear Regression model that accurately predicts **car prices** based on the given input features and evaluate its performance using standard regression metrics.

---

## Approach
* Loaded the `Train.csv` and `Test.csv` datasets and inspected features such as **Year**, **KilometersDriven**, **Mileage**, **Engine**, **Power**, **Seats**, and **Price**
* Preprocessed the data by:
  * Extracting numeric values from string-based features with units (e.g., `"23.84 kmpl"`, `"1199 CC"`, `"84 bhp"`)
  * Handling missing values by dropping or cleaning affected rows
* Applied mean normalization / standardization to selected numerical features to improve gradient descent convergence
* Implemented Linear Regression **from scratch using NumPy**, manually defining weights, bias, and gradient descent updates
* Tracked the cost function (MSE) across iterations and evaluated the trained model on the test set using **MSE**, **RMSE**, and **R² score**

---

## Key Concepts Explored
* Linear relationships between car features *(year, usage, mileage, engine size, power, seats)* and target price
* Implementation of the Mean Squared Error (MSE) cost function and its minimization using gradient descent
* Importance of feature scaling for stable and faster optimization
* Regression evaluation metrics: interpreting **RMSE** and **R² score** for unseen data
* Underfitting vs overfitting and limitations of linear regression models

---

## Tools & Libraries
* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn *(used only for evaluation/verification)*

---

## Key Learnings
This project provided hands-on experience in building a regression model from the ground up, cleaning real-world tabular data, and evaluating model performance using appropriate regression metrics.

---

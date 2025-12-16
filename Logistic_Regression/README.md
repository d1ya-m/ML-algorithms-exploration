# Logistic Regression From Scratch

## Overview
This project implements **Logistic Regression from scratch using Gradient Descent** to solve a binary classification problem on a structured tabular dataset. The focus is on understanding probability-based classification and how linear decision boundaries are learned.


## Project Structure
```
.
├── Gotem-Pumpkins-train.csv
├── Freyja_Pumpkins-test.csv
├── logistic_regression.ipynb
└── README.md
```
---

## Dataset
The dataset consists of pumpkin samples described by multiple features and a binary class label.

**Target variable:** Pumpkin label (binary class)
**Input features:** Numerical and/or encoded attributes describing each pumpkin (e.g., size, shape, color/intensity-related features)

The training dataset is used to learn model parameters, while the test dataset is used to evaluate generalization performance.

---

## Problem Statement
To build a Logistic Regression model that predicts the **binary class of a pumpkin** based on input features and evaluate its performance using standard classification metrics.

---

## Approach
* Loaded and explored the training and test datasets to understand features and labels
* Performed data preprocessing including handling missing values and selecting relevant numeric features
* Applied feature scaling to ensure stable and efficient gradient descent
* Implemented Logistic Regression **from scratch using NumPy**, including:
  * Sigmoid activation for probability estimation
  * Binary cross-entropy (log-loss) as the cost function
  * Gradient descent for updating weights and bias
* Trained the model on the training set and evaluated it on the test set

---

## Evaluation Metrics
* Accuracy
* Precision
* Recall
* F1-score
* (Optional) ROC–AUC

---

## Key Concepts Explored
* Probabilistic classification using the sigmoid function
* Optimization of binary cross-entropy loss via gradient descent
* Effect of feature scaling on convergence speed
* Interpretation of classification metrics beyond accuracy
* Limitations of linear decision boundaries in logistic regression

---

## Tools & Libraries
* Python
* NumPy
* Pandas
* Matplotlib / Seaborn

---

## Key Learnings
This project provided hands-on experience with building a classification model from the ground up, understanding how probabilities are estimated, and evaluating model performance on unseen data.

---


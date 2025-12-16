# Bagging & Boosting (AdaBoost)

## Overview
This project applies **ensemble learning techniques—Bagging and AdaBoost—** to a large tabular **Threats** classification dataset. The objective is to analyze how ensemble models built on top of decision trees improve predictive performance, robustness, and generalization compared to a single decision tree.

---

## Project Structure
```
.
├── Threats (1).csv
├── bagging_adaboost.ipynb
└── README.md
```

---

## Dataset
**File:** `Threats (1).csv`

Each row represents a single threat or event instance described by multiple **categorical and numerical attributes**, along with a target label indicating the threat type or severity class.

**Input features:**
Identifiers, timestamps, technical indicators, and contextual attributes (categorical and numeric)

**Target variable:**
Threat label / class

All feature columns are used as inputs to the ensemble models, while the target label supervises training.

---

## Problem Statement
To build and compare **Bagging** and **AdaBoost** classifiers for predicting the threat label of each instance, and to evaluate how these ensemble strategies differ in performance and behavior relative to a single Decision Tree.

---

## Approach
* Loaded and explored `Threats (1).csv` to inspect feature types, class distribution, and data quality
* Preprocessed the dataset by:
  * Handling missing or inconsistent values
  * Encoding categorical variables using label or one-hot encoding
  * Splitting the data into training and testing sets
* Trained a **baseline Decision Tree classifier** to serve as a reference model
* Built two ensemble models using scikit-learn:
  * **BaggingClassifier** with decision trees as base estimators (bootstrap sampling + majority voting)
  * **AdaBoostClassifier** with shallow decision trees as weak learners, updating sample weights across boosting iterations
* Evaluated the baseline tree, Bagging model, and AdaBoost model using **accuracy**, **precision**, **recall**, **F1-score**, and confusion matrices, and compared their results

---

## Key Concepts Explored
* **Bagging (Bootstrap Aggregating):** reducing variance and overfitting by training multiple models on bootstrapped samples and aggregating predictions
* **AdaBoost:** sequentially focusing on misclassified samples to reduce bias and build a strong classifier from weak learners
* Effect of ensemble hyperparameters such as number of estimators, tree depth, and learning rate (AdaBoost)
* Comparison of single-model vs ensemble performance on high-dimensional, real-world datasets
* Interpretation of classification metrics and confusion matrices for ensemble models

---

## Tools & Libraries
* Python
* NumPy
* Pandas
* Scikit-learn
* Matplotlib / Seaborn

---

## Key Learnings

This project provided hands-on experience with ensemble learning, highlighting how Bagging and AdaBoost improve robustness and performance over single decision trees when applied to complex classification problems.

---

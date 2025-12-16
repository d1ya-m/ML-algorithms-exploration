# Decision Trees

## Overview
This project applies **Decision Tree classifiers** to perform supervised classification on a large tabular **Threats** dataset. The objective is to learn **human-interpretable decision rules** that classify each record into the correct threat category based on its attributes.

---

## Project Structure
```
.
├── Threats (1).csv
├── decision_tree.ipynb
└── README.md
```

---

## Dataset
**File:** `Threats (1).csv`

Each row represents a single threat or event instance described by multiple **categorical and numerical features**, along with a target label indicating the threat type or class.

**Input features:**
Identifiers, timestamps, technical attributes, and contextual fields (categorical and numeric)

**Target variable:**
Threat label / class

All feature columns are used as inputs to the model, while the target label supervises training.

---

## Problem Statement
To build a Decision Tree classifier that accurately predicts the **threat label** for each instance based on its feature values, and to analyze the learned tree structure to understand **feature importance and decision rules**.

---

## Approach
* Loaded and explored `Threats (1).csv` to inspect feature types, class distribution, and data quality
* Preprocessed the dataset by:
  * Handling missing or noisy values
  * Encoding categorical features using label or one-hot encoding
  * Splitting the data into training and testing sets
* Trained a **DecisionTreeClassifier** using scikit-learn with controlled hyperparameters such as:
  * Maximum depth
  * Minimum samples per split / leaf
  * Splitting criterion (Gini index or entropy)
* Evaluated model performance on the test set using **accuracy**, **precision**, **recall**, **F1-score**, and a confusion matrix
* Visualized or inspected the learned tree and feature importances to interpret model decisions

---

## Key Concepts Explored
* Supervised classification using **Decision Trees** and recursive feature-based splitting
* Impurity measures (**Gini index** and **entropy**) and their role in split selection
* Overfitting in tree-based models and regularization through depth and sample constraints
* Interpreting confusion matrices and classification metrics on complex, real-world data
* Trade-off between model interpretability and generalization

---

## Tools & Libraries
* Python
* NumPy
* Pandas
* Scikit-learn
* Matplotlib / Seaborn

---

## Key Learnings
This project provided practical experience in training and interpreting decision tree models, understanding feature importance, and managing overfitting in supervised classification tasks on large, mixed-type datasets.

---

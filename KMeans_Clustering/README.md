# Clustering (K-Means)

## Overview
This project applies **unsupervised clustering techniques** to group similar wine-like samples from a structured tabular dataset. The objective is to discover natural groupings based on chemical composition and understand how clustering algorithms organize **unlabeled data**.

---

## Project Structure
```
.
├── Clustering_Data.csv
├── clustering.ipynb
└── README.md
```

---

## Dataset
**File:** `Clustering_Data.csv`

Each row represents a single sample described by chemical analysis attributes, along with an existing segment label used only for evaluation and interpretation.

### Features
* `Alcohol` — Alcohol content
* `Malic_Acid` — Concentration of malic acid
* `Ash` — Total ash content
* `Ash_Alcanity` — Alkalinity of ash
* `Magnesium` — Magnesium content
* `Total_Phenols` — Total phenolic compounds
* `Flavanoids` — Flavonoid phenol content
* `Nonflavanoid_Phenols` — Non-flavonoid phenol content
* `Proanthocyanins` — Proanthocyanin concentration
* `Color_Intensity` — Color intensity
* `Hue` — Hue of the sample
* `OD280` — OD280/OD315 of diluted wines (phenol-related measure)
* `Proline` — Proline concentration

**Additional column (not used for training):**
* `Customer_Segment` — Existing class/segment label (used only for evaluation and visual comparison)

**What is clustered:**
Each sample is treated as a point in a **13-dimensional feature space** formed by the chemical attributes (excluding `Customer_Segment`).

---

## Problem Statement
To build clustering models that automatically group samples based on similarity in chemical features, and to analyze how the resulting clusters relate to the known `Customer_Segment` labels.

---

## Approach
* Loaded and explored `Clustering_Data.csv` to analyze distributions and relationships among chemical attributes
* Applied feature scaling / standardization so that all attributes contribute equally to distance-based clustering
* Implemented **K-Means clustering** to partition samples into a chosen number of clusters
* Used methods such as the **elbow method** and **silhouette score** to guide selection of the optimal number of clusters
* Visualized clusters in 2D (using PCA or selected feature pairs) and compared them with `Customer_Segment` labels to interpret alignment between unsupervised clusters and known classes

---

## Key Concepts Explored
* Unsupervised learning and how it differs from supervised classification
* **K-Means clustering**: centroid initialization, assignment and update steps, and convergence
* Importance of **feature scaling** for distance-based algorithms
* Cluster evaluation using inertia (within-cluster sum of squares), elbow plots, and silhouette scores
* Interpreting clusters by comparing them with known segment labels

---

## Tools & Libraries
* Python
* NumPy
* Pandas
* Scikit-learn
* Matplotlib / Seaborn

---

## Key Learnings
This project provided hands-on experience with unsupervised learning, selecting the number of clusters, and interpreting clustering results in the context of real-world chemical feature data.

---

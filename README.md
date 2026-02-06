# 🌲 Random Forest Regressor: Advanced Prediction Analysis

This repository contains a comprehensive implementation of the **Random Forest Regressor**, focusing on predicting continuous values while managing model complexity. The project demonstrates the use of ensemble learning to improve predictive performance and generalization.

## 🚀 Project Overview

The objective of this project is to implement a robust Random Forest model that avoids "memorization" (overfitting) by carefully tuning hyperparameters. By averaging the results of multiple decision trees, the model achieves more stable and reliable predictions compared to a single estimator.

### Key Highlights:
* **Controlled Complexity:** Implemented `max_depth` and `min_samples_leaf` constraints to prevent deep overfitting.
* **Feature Randomness:** Used `max_features='sqrt'` to ensure each split considers only a subset of features, increasing the diversity of the trees.
* **Metric Evaluation:** Comprehensive evaluation using **R² Score**, **Mean Absolute Error (MAE)**, and **Mean Squared Error (MSE)**.

## 🛠️ Tech Stack

* **Language:** Python
* **Libraries:** Scikit-Learn, Pandas, NumPy
* **Algorithm:** Random Forest Regressor

---

## 📊 Model Performance

The model was evaluated on both training and testing datasets to monitor generalization.

### 1. Regression Metrics
| Metric | Training Set | Testing Set |
| :--- | :--- | :--- |
| **R² Score** | **0.5538** | **0.4674** |
| **Mean Absolute Error (MAE)** | 43.87 | — |
| **Mean Squared Error (MSE)** | 2847.73 | 3062.46 |

### 2. Tuning Insights
The results show a balanced $R^2$ score between training and testing, indicating that the regularization parameters (like `min_samples_leaf=15`) effectively reduced the gap between training and real-world performance.

---

## 📂 Repository Structure

* `Random_Forest_Regressor.ipynb`: The main Jupyter Notebook containing the data preprocessing, model training, and performance evaluation.


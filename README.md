# 🎓 Student Performance Stacking

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-%23EB4034.svg?style=for-the-badge&logo=xgboost&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 🚀 Overview

**Student Performance Stacking** is a machine learning project designed to predict student outcomes based on their learning habits, demographics, and engagement metrics. 

Unlike simple regression models, this project leverages a **Stacking Ensemble** architecture, combining the strengths of **Random Forest**, **XGBoost**, and **Gradient Boosting** to achieve superior prediction accuracy for both:
1.  **Regression:** Predicting the exact Final Exam Score.
2.  **Classification:** Predicting the Pass/Fail status.

## 📊 Dataset

The model is trained on the **Python Learning & Exam Performance Dataset** (3,000 synthetic samples), which includes granular features such as:
* **Engagement:** `hours_spent_learning`, `videos_watched`, `debugging_sessions`.
* **Active Learning:** `projects_completed`, `practice_problems_solved`.
* **Community:** `uses_kaggle`, `forum_participation`.

> **Note:** The dataset source is available on [Kaggle](https://www.kaggle.com/).

## 🧠 Model Architecture

This project implements a robust **Stacking Ensemble** pipeline:

1.  **Level 0 (Base Learners):**
    * Random Forest Regressor (captures complex non-linear patterns).
    * XGBoost Regressor (gradient boosting for high performance).
    * Gradient Boosting Regressor (minimizes bias).
2.  **Level 1 (Meta-Learner):**
    * Ridge Regression (learns how to best combine the predictions of the base learners).

All models are wrapped in a **Scikit-Learn Pipeline** to ensure clean data processing and prevent data leakage.

## 🛠️ Key Features

* **Advanced Preprocessing:** Automated `ColumnTransformer` for missing value imputation, One-Hot Encoding for categorical data, and Standard Scaling for numerical data.
* **EDA & Visualization:** Comprehensive analysis of "Effort vs. Outcome" using Seaborn (Violin plots, Correlation Matrices).
* **Leakage Prevention:** Strict separation of target variables (`final_exam_score`) during classification tasks.

## 📈 Results
| **Accuracy** | XGBoost Classifier | *90%* |

*(Note: Replace the placeholders above with your actual notebook results)*
#  [Shenouda Safwat](https://www.linkedin.com/in/shenouda-safwat/)

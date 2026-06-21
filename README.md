# Codveda Technology — Machine Learning Internship

This repository contains my completed tasks for the Machine Learning
internship at **Codveda Technology**, covering data preprocessing,
regression, classification, and ensemble methods across all three
difficulty levels.

## About Codveda
Codveda Technology specializes in web development, app development,
digital marketing, SEO optimization, AI/ML automation, and data
analysis — helping businesses unlock their potential through
innovative, scalable solutions. [codveda.com](https://www.codveda.com)

## Intern Details
- **Name:** Sachin Singh
- **Domain:** Machine Learning
- **Program:** Codveda Internship — 1 month

## Tasks Completed (2 per level, as required)

### Level 1 — Basic
| Task | Description | Folder |
|---|---|---|
| 1 | Data Preprocessing for Machine Learning | [`task1_data_preprocessing`](./task1_data_preprocessing) |
| 2 | Simple Linear Regression Model | [`task2_linear_regression`](./task2_linear_regression) |

### Level 2 — Intermediate
| Task | Description | Folder |
|---|---|---|
| 1 | Logistic Regression for Binary Classification | [`task3_logistic_regression`](./task3_logistic_regression) |
| 2 | Decision Trees for Classification | [`task4_decision_trees`](./task4_decision_trees) |

### Level 3 — Advanced
| Task | Description | Folder |
|---|---|---|
| 1 | Random Forest Classifier | [`task5_random_forest`](./task5_random_forest) |
| 2 | Support Vector Machine (SVM) for Classification | [`task6_svm`](./task6_svm) |

## Summary of Results

| Task | Model | Dataset | Key Metric |
|---|---|---|---|
| 1 | Preprocessing | Titanic | 891 → 0 missing values |
| 2 | Linear Regression | California Housing | R² = 0.576 |
| 3 | Logistic Regression | Telco Customer Churn | AUC = 0.842 |
| 4 | Decision Tree | Iris | Accuracy = 96.7% |
| 5 | Random Forest | Telco Customer Churn | F1 = 0.628 (tuned) |
| 6 | SVM | Breast Cancer Wisconsin | AUC = 0.996 (linear) |

## Key Learnings
- End-to-end ML workflow: cleaning, encoding, scaling, training, evaluation
- Why metric choice matters more than raw accuracy on imbalanced data
  (Tasks 3 & 5 — precision/recall/F1 vs accuracy)
- Bias-variance tradeoff in practice: pruning decision trees (Task 4)
  and hyperparameter tuning Random Forest (Task 5) to reduce overfitting
- Kernel choice in SVM and when flexibility (RBF) helps vs a simpler
  linear boundary (Task 6)
- Interpreting models two ways: coefficients/odds ratios (logistic
  regression) vs feature importance (Random Forest) — and how both
  pointed to the same underlying churn drivers

## Tools & Technologies
Python, pandas, NumPy, scikit-learn, matplotlib, seaborn, Google Colab

## Connect
- GitHub: [@BUGHUNTER-SACHIN](https://github.com/BUGHUNTER-SACHIN)

---
*#CodvedaJourney #CodvedaExperience #FutureWithCodveda*

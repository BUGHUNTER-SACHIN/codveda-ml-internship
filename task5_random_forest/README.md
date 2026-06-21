# Task 5: Build a Random Forest Classifier

## Objective
Implement a Random Forest model for classification on a complex dataset.

## Dataset
Telco Customer Churn dataset (7,043 customers, 30 features after encoding)

## Steps Performed
- Reused cleaned/encoded data from Task 3 (no scaling needed - tree-based model)
- Trained a baseline Random Forest model
- Tuned hyperparameters (n_estimators, max_depth, min_samples_split,
  class_weight) using GridSearchCV with 5-fold cross-validation, optimizing for F1-score
- Evaluated tuned model using accuracy, precision, recall, F1-score, and confusion matrix
- Performed feature importance analysis

## Results
- Baseline: Accuracy 78.6%, F1-score 0.550
- Tuned: Accuracy 76.7%, Precision 54.4%, Recall 74.3%, F1-score 0.628
- 5-fold CV F1: 0.644 (+/- 0.020)
- Best params: n_estimators=100, max_depth=10, min_samples_split=5,
  class_weight='balanced'

## Key Insight
Using class_weight='balanced' to address the dataset's class imbalance
significantly improved recall (55.9% -> 74.3% compared to the Task 3
logistic regression model), at the cost of precision. This is a better
tradeoff when the business cost of missing a churner outweighs the cost
of a false retention offer. Top predictive features (tenure, contract
length, internet service type) align closely with the logistic
regression findings from Task 3, reinforcing that these are genuine
churn drivers rather than model-specific artifacts.

## Tools Used
Python, pandas, scikit-learn, matplotlib, NumPy

## Files
- `Codveda_Task5_Random_Forest.ipynb` — full notebook with code,
  hyperparameter tuning, and feature importance visualization

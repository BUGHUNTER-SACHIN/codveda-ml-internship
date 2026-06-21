# Task 3: Logistic Regression for Binary Classification

## Objective
Implement a logistic regression model to predict binary outcomes
(customer churn).

## Dataset
Telco Customer Churn dataset (7,043 customers, 31 features after encoding)
Class distribution: 73% No Churn / 27% Churn

## Steps Performed
- Cleaned data (fixed TotalCharges data type, handled 11 missing values)
- Encoded target variable and 15 categorical features (one-hot encoding)
- Split data with stratification to preserve class balance
- Scaled numerical features (tenure, MonthlyCharges, TotalCharges)
- Trained a Logistic Regression model using scikit-learn
- Interpreted coefficients as odds ratios
- Evaluated using accuracy, precision, recall, and ROC-AUC

## Results
- Accuracy: 80.6%
- Precision: 65.7%
- Recall: 55.9%
- AUC: 0.842

## Key Insight
Contract type and tenure are the strongest predictors of churn.
Customers on month-to-month contracts, with low tenure, and fiber-optic
internet are highest risk. The model has higher precision than recall —
it misses some actual churners (165 false negatives vs 109 false
positives), which matters in a real retention use case where missing
a churner is costlier than a false alarm.

## Tools Used
Python, pandas, scikit-learn, matplotlib, NumPy

## Files
- `Codveda_Task3_Logistic_Regression.ipynb` — full notebook with code,
  outputs, and ROC curve visualization

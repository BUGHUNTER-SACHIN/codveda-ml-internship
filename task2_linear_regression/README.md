# Task 2: Build a Simple Linear Regression Model

## Objective
Build a linear regression model to predict a continuous variable (house prices).

## Dataset
California Housing dataset (20,640 samples, 8 features) — built into scikit-learn

## Steps Performed
- Loaded and explored the dataset (no missing values)
- Split data into training (80%) and testing (20%) sets
- Trained a Linear Regression model using scikit-learn
- Interpreted model coefficients (e.g., median income and location were strongest predictors)
- Evaluated performance using R-squared and Mean Squared Error (MSE)
- Visualized predicted vs actual values

## Results
- R-squared: 0.576 (model explains ~58% of variance in house prices)
- RMSE: ~$74,600

## Key Insight
Linear regression captures the general price trend but underperforms at the
high end of the price range, partly due to the dataset's $500k value cap
and non-linear pricing dynamics (location, market behavior) that a linear
model can't fully capture. Also observed multicollinearity between
AveRooms and AveBedrms, which caused unstable/counterintuitive coefficients.

## Tools Used
Python, pandas, scikit-learn, matplotlib, NumPy

## Files
- `Codveda_Task2_Linear_Regression.ipynb` — full notebook with code, outputs, and visualizations

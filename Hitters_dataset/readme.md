# Hitters Salary Prediction

Predicting baseball players' salaries using Ridge, Lasso, and OLS Regression.

## Steps
1. Data cleaning and imputation of missing salary values.
2. Outlier detection and removal.
3. One-hot encoding of categorical features.
4. Feature scaling with StandardScaler.
5. Model training using Ridge, Lasso, and OLS regression.
6. Evaluation using R² and MSE.

## Results
- **Ridge R²:** 0.3057 | **MSE:** 101724.16  
- **Lasso R²:** 0.2615 | **MSE:** 108191.54  
- **OLS R²:** 0.4210

## Conclusion
Ridge regression achieved better generalization than Lasso, while OLS gave the best R² fit.  
Regularization proved effective for managing model variance.

## Libraries
Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Statsmodels

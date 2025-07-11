# Lab 4: Regression and Regularization on the Diabetes Dataset

**Author:** Jacob Jeffers  
**Course:** MSCS 634 – Data Mining  

## Overview
This lab focused on exploring multiple regression techniques using the Diabetes dataset from `sklearn.datasets`. I implemented various regression models, from simple linear regression to more advanced techniques like Ridge and Lasso, to analyze disease progression based on health measurements. I also evaluated the models using common metrics and visualized the results to better understand performance differences.

## What I Did
- Loaded and explored the Diabetes dataset
- Built a simple linear regression model using BMI as the independent variable
- Expanded to multiple regression using all features
- Applied polynomial regression with degree 2
- Used Ridge and Lasso regression to apply regularization
- Evaluated each model using MAE, MSE, RMSE, and R²
- Visualized actual vs. predicted outcomes to compare model fit

## Key Results
- **Simple Linear Regression (BMI only)**:  
  R² = 0.36 — showed a decent correlation but limited predictive power

- **Multiple Linear Regression**:  
  R² = 0.45 — captured more variation in the target by including more features

- **Polynomial Regression (degree 2)**:  
  R² = 0.53 — improved the fit but risked overfitting

- **Ridge Regression (alpha=1.0)**:  
  R² = 0.46 — helped with overfitting by penalizing large coefficients

- **Lasso Regression (alpha=0.1)**:  
  R² = 0.45 — slightly underperformed compared to Ridge but offered model simplicity

## Insights and Observations
- Polynomial regression improved performance over linear models but could overfit without regularization
- Ridge regression provided the best balance of fit and generalization
- Lasso was helpful for feature selection but slightly less accurate in this case
- The Diabetes dataset has moderate complexity and benefits from regularization

## Challenges Faced
Most of the lab went smoothly. One challenge was choosing the right alpha values for Ridge and Lasso. It was also interesting to observe how visualizing predictions helped reinforce the numerical evaluation metrics.

## Files Included
- `lab4.ipynb`: Full Jupyter notebook with code, evaluation, and visualizations
- `README.md`: Summary of work and insights

# Experiment Summary

This project groups three regression-focused machine learning experiments into one clean portfolio repository.

## 1. Simple Linear Regression

- Dataset: population vs. food-truck profit
- Implementation: custom NumPy linear regression
- Optimization: batch gradient descent
- Initial cost: approximately `32.07`
- Example predictions:
  - Population value `3.5`: approximately `0.393`
  - Population value `7.0`: approximately `4.507`
- Compared custom parameters with scikit-learn `LinearRegression`.

## 2. Multiple Linear Regression

- Dataset: house size, number of bedrooms, and house price
- Applied feature normalization before gradient descent.
- Compared learning rates: `0.01`, `0.05`, and `0.1`.
- Predicted price for a 1650-square-foot house with 3 bedrooms:
  - Gradient descent result: approximately `293214`
  - Normal equation result: approximately `293081`
- Compared custom workflow with scikit-learn preprocessing and regression.

## 3. Nonlinear Kernel Regression

- Dataset: housing-price data
- Implemented Gaussian-kernel regression using the Nadaraya-Watson estimator.
- Explored how the gamma hyperparameter changes predictions.
- Example prediction for `[1650, 3]`: approximately `303396`
- Evaluated a scikit-learn `KernelRidge` model using mean squared error.
- Test MSE shown in notebook output: approximately `6.84e9`.

## Portfolio Value

This repository demonstrates machine learning fundamentals and supports more advanced portfolio projects by showing that the core regression algorithms, evaluation steps, and optimization logic are understood from the ground up.

# Post-COVID: A Comparison of Regularization in Linear Regression and Neural Networks
Authors: Elena Muyo de Bonrostro, Colby Eagan, Julia Katsoulis, Charles Moseley, Joseph Sachtleben

Course: STOR 565 – Department of Statistics and Operations Research, UNC-Chapel Hill

**Overview**

This project predicts NCAA men’s basketball win percentages in the post-COVID era using statistical and machine learning models. We compare L1 (Lasso), L2 (Ridge), and Dropout-Regularized Neural Networks to evaluate their predictive performance and interpretability.
The motivation stems from changes in the college basketball landscape — the transfer portal, NIL policies, and extended eligibility — which altered historical patterns, making regularization and robust modeling increasingly important.

**Data**

Source: Kaggle NCAA basketball datasets (2022–2025 seasons)
Preprocessing:
Standardized team names
Removed redundant/postseason variables
Engineered win percentage variable
One-hot encoded categorical conference variable
Z-score normalization applied before modeling

**Methods**

L1 Regularization (Lasso): Feature selection + coefficient shrinkage
L2 Regularization (Ridge): Coefficient shrinkage for generalization
Neural Network (PyTorch): Feedforward model with two hidden layers, ReLU activation, and dropout
Evaluation Metrics: MSE, RMSE, MAE, R², plus residual and Q-Q plots

**Results**

Lasso (α=0.01): R² ≈ 0.804, RMSE ≈ 0.074

LassoCV (α=0.0003): R² ≈ 0.845, RMSE ≈ 0.066

Ridge (α=0.01): R² ≈ 0.842, RMSE ≈ 0.067 *RidgeCV performed the same

Neural Network: R² ≈ 0.860, RMSE ≈ 0.063

Key Predictors Identified: Strength of Schedule (SOS_Rating), Adjusted Offensive Efficiency (ADJOE), Adjusted Defensive Efficiency (ADJDE), Effective Field Goal % (Offense & Defense), Turnover Rates

**Insights**

Neural networks captured complex, nonlinear interactions and achieved the best accuracy.
Linear models remained competitive and offered interpretability through coefficients.
Tradeoff: interpretability (Lasso, Ridge) vs predictive power (Neural Network).

**Skills Demonstrated**

Data cleaning & feature engineering
Regularization methods (Lasso, Ridge)
Neural network modeling with PyTorch
Cross-validation & hyperparameter tuning
Model diagnostics (residual plots, Q-Q plots)
Balancing interpretability vs predictive accuracy

**Files**

lasso_ridge_models.ipynb – Python code for Lasso and Ridge regression

neural_network.ipynb – Python code for neural network implementation

post_covid_basketball_report.pdf – Full written report (includes visuals & analysis)

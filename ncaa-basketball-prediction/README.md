# NCAA Basketball Win Prediction


This project predicts NCAA men’s basketball win percentages using multiple statistical and machine learning models. The analysis compares model performance and identifies the most influential predictors of team success.

**Overview**


Using NCAA basketball season data (2022–2025), this project explores how offensive, defensive, and schedule-related statistics affect team win percentages. Models used include:
1. LASSO Regression
2. Ridge Regression
3. Neural Network
The goal was to compare predictive accuracy and interpretability across methods.

**Data**
Source: Kaggle NCAA Men’s Basketball datasets (adjusted for post-COVID seasons)
Variables: Effective Field Goal Percentage (Offense & Defense), Turnover Rates, Offensive Rebounds, Strength of Schedule, Adjusted Offensive/Defensive Efficiency, and others.
Preprocessing:
Standardized team names
Removed redundant variables
Calculated win percentages
One-hot encoded conference variable

**Methods & Tools**
Languages: Python
Libraries: pandas, NumPy, scikit-learn, matplotlib, ggplot2, dplyr, caret
Techniques: Data cleaning, exploratory data analysis, LASSO & Ridge regression, neural network modeling, cross-validation, residual analysis, Q-Q plots

**Results**
Best Model: LASSO with Cross-Validation (R² = 0.8446, RMSE = 0.066)
Top Predictors: Strength of Schedule (SOS_Rating), Adjusted Offensive Efficiency (ADJOE), Adjusted Defensive Efficiency (ADJDE), Effective Field Goal % (Offense & Defense)
Key Insights:
Teams with stronger offensive efficiency and better shooting tend to win more.
Higher strength of schedule can negatively impact win percentage due to tougher opponents.

**Skills Demonstrated**
Data preprocessing & feature engineering
Regularization techniques (L1, L2)
Neural network implementation
Model comparison using R², RMSE, MAE
Visualization & interpretation of model diagnostics

**Files**
data_cleaning.R – Prepares and cleans dataset
modeling_lasso_ridge.R – Fits LASSO & Ridge models
neural_network.py – Fits and evaluates neural network model
plots/ – Residual plots, Q-Q plots, and predictor importance charts

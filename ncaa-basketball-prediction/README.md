# Predicting NCAA Men's Basketball Win Percentages Post-COVID

This project analyzes NCAA men’s basketball seasons (2022–2025) to predict team win percentages in the post-COVID era, where policy changes like the transfer portal, NIL, and extended eligibility reshaped historical patterns. Using Kaggle datasets, we cleaned and engineered features (standardized team names, one-hot encoded conferences, created win percentage, applied z-score normalization) before applying Lasso (L1), Ridge (L2), and a dropout-regularized neural network. Models were tuned via cross-validation and evaluated with MSE, RMSE, MAE, and R². Results showed the neural network achieved the best accuracy (R² ≈ 0.86, RMSE ≈ 0.063), while Lasso and Ridge remained competitive and offered interpretability by identifying key predictors such as strength of schedule, offensive/defensive efficiency, and turnover rates. This work highlights the tradeoff between predictive power and interpretability, and demonstrates skills in data preprocessing, regularization, neural network modeling with PyTorch, and model diagnostics.

**Files**

lasso_ridge_models.ipynb – Python code for Lasso and Ridge regression

neural_network.ipynb – Python code for neural network implementation

post_covid_basketball_report.pdf – Full written report (includes visuals & analysis)

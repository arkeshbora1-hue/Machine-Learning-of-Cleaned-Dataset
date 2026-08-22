# Machine-Learning-of-Cleaned-Dataset
Predicts used car resale prices in India with Linear Regression and Random Forest models. Includes EDA, log-transformation, IQR outlier removal, one-hot encoding, and Random Forest hyperparameter tuning via GridSearchCV, evaluated using MAE, RMSE, and R².
Overview

Starting from a cleaned used-car listings dataset, this project builds and compares regression models to predict car price based on features such as engine size, mileage, kilometers driven, fuel type, transmission, ownership history, and city.

Key Steps
Exploratory Data Analysis – price distribution, fuel-type comparisons, correlation heatmaps, joint/KDE plots, pair plots, and facet grids
Baseline Modeling – Linear Regression as a starting benchmark
Advanced Modeling – Random Forest Regressor for improved accuracy
Target Transformation – log-transforming Price_INR to address skew and heteroscedasticity
Outlier Handling – IQR-based outlier detection and removal
Hyperparameter Tuning – GridSearchCV for optimizing the Random Forest model
Feature Encoding – one-hot encoding of categorical variables (Fuel Type, Transmission, Owner, City)
Model Evaluation – MAE, RMSE, and R² score, plus residual analysis and actual-vs-predicted visualizations
Models Compared
Model	Notes
Linear Regression	Baseline model
Linear Regression (log target)	Applied to reduce skew in price
Random Forest Regressor	Non-linear baseline
Random Forest (log target)	Improved residual behavior
Random Forest (tuned, log target)	Best-performing model via GridSearchCV
Tech Stack
Python
pandas, NumPy
scikit-learn
Matplotlib, Seaborn

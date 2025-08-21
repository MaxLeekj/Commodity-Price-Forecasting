# Commodity-Price-Forecasting
## PVC_ARIMAX_forecast

### Overview

This repository contains a Jupyter Notebook for forecasting Polyvinyl Chloride (PVC) prices using advanced time-series modeling. The workflow leverages the ARIMAX (AutoRegressive Integrated Moving Average with eXogenous variables) model, incorporating external explanatory variables to improve forecast accuracy.

### Features

- **Data Preprocessing:** Cleans and normalizes historical PVC pricing and feature data.
- **Feature Selection:** Identifies influential features using correlation analysis and ElasticNet regression.
- **Stationarity Check:** Applies the Augmented Dickey-Fuller (ADF) test for time series suitability.
- **Model Order Identification:** Uses autocorrelation (ACF) and partial autocorrelation (PACF) plots to guide ARIMAX hyperparameter selection.
- **Train/Test Split:** Splits data into training and test sets (last 12 months for out-of-sample evaluation).
- **Baseline and Tuned ARIMAX Models:** Trains a baseline ARIMAX model and performs grid search hyperparameter tuning (AIC optimization).
- **Forecasting and Visualization:** Generates forecasts with confidence intervals and visualizes actual vs. predicted values, including uncertainty bands.
- **Unnormalized Results:** All final visualizations and metrics are displayed in original PVC price units for interpretability.
- **Model Diagnostics:** Includes residual analysis, confidence interval diagnostics, and coverage statistics.

# PVC Price Feature Selection and Correlation Analysis

## Overview

This repository contains a Jupyter Notebook for feature selection and correlation analysis to support PVC price forecasting. The notebook applies multiple statistical and machine learning methods to identify the most impactful predictors from a raw dataset, laying the foundation for robust time-series modeling.

## Key Features

- **Correlation Analysis:**  
  Calculates the statistical relationship between each feature and the target variable to identify strong linear associations.

- **XGBoost Feature Importance:**  
  Uses the XGBoost algorithm to evaluate feature importance based on how frequently and effectively features are used for data splits in decision trees, capturing both linear and non-linear relationships.

- **Random Forest Feature Importance:**  
  Applies Random Forest to measure feature importance via impurity reduction, making it robust to outliers and able to capture complex feature interactions.

- **ElasticNet Regression:**  
  Uses ElasticNet to determine feature importance by evaluating model coefficients, effectively handling multicollinearity among predictors.

- **Lagged Feature Engineering:**  
  Shifts predictor variables by one or more time periods to uncover delayed relationships with the target variable, which is essential for accurate time-series forecasting.

- **Data Normalization:**  
  Normalizes features using MinMaxScaler and StandardScaler to optimize correlation calculations and ensure comparability across methods.

- **Visualization:**  
  Provides clear bar plots of feature importances for each method, helping users quickly identify top predictors.

- **Multicollinearity Handling:**  
  Includes logic to select uncorrelated features, improving model interpretability and performance.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook
- pandas, numpy, matplotlib, seaborn
- scikit-learn, xgboost

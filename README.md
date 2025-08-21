# Commodity-Price-Forecasting
PVC_ARIMAX_forecast
Overview
This repository contains a comprehensive Jupyter Notebook for forecasting Polyvinyl Chloride (PVC) prices using advanced time-series modeling techniques. The workflow leverages the ARIMAX (AutoRegressive Integrated Moving Average with eXogenous variables) model, which extends ARIMA by incorporating external explanatory variables to improve forecast accuracy.

Main Features
Data Preprocessing:
Cleans and normalizes historical PVC pricing and relevant feature data.
Feature Selection:
Identifies the most influential features using correlation analysis and ElasticNet regression.
Stationarity Check:
Applies the Augmented Dickey-Fuller (ADF) test to ensure the time series is suitable for ARIMAX modeling.
Model Order Identification:
Uses autocorrelation (ACF) and partial autocorrelation (PACF) plots to guide the selection of ARIMAX hyperparameters.
Train/Test Split:
Splits the data into training and test sets, typically with the last 12 months reserved for out-of-sample evaluation.
Baseline and Tuned ARIMAX Models:
Trains a baseline ARIMAX model and performs hyperparameter tuning via grid search to optimize performance (using AIC).
Forecasting and Visualization:
Generates forecasts with confidence intervals and visualizes actual vs. predicted values, including uncertainty bands and coverage analysis.
Unnormalized Results:
All final visualizations and metrics are displayed in original (unnormalized) PVC price units for interpretability.
Model Diagnostics:
Includes residual analysis, confidence interval diagnostics, and coverage statistics for robust model validation.

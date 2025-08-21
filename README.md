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

### Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git

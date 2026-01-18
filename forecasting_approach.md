# Forecasting Objective

The objective of this project was to forecast short-term sales for a low-calorie ice-cream product (WISP) across five UK regions, in order to support:

- Inventory planning

- Marketing budget allocation

- Regional demand planning

The analysis combines marketing impact modelling with time-series forecasting, recognising that sales are driven by both promotional activity and seasonality.

# Key Forecasting Challenges

- Extremely small dataset (36 observations per region)

- Strong seasonality and trend components

- Presence of outliers (notably December 2018)

- Inability of ARIMA models to incorporate external shocks

These constraints required a careful, assumption-driven forecasting strategy rather than aggressive optimisation.

# Forecasting Strategy Overview

The approach consisted of three analytical layers:

1. Marketing Impact Modelling (Regression Layer)

- Sales were log-transformed to stabilise variance

- Multiple Linear Regression used to quantify:

   - TV Ads

   - Banners

   - Promotions

- Model validation:

  - Adjusted R² ≈ 0.97

  - Residual Standard Error ≈ 6.2%

📌 Purpose:

Understand drivers of demand, not forecasting directly.

2. Time-Series Preparation

- Region-wise time series created

- Stationarity tested using ADF test

- Non-stationary series differenced iteratively

- Seasonal and trend effects isolated

📌 Purpose:

Ensure statistical validity before forecasting.

3. ARIMA-Based Forecasting

- ACF and PACF plots used to select (p, d, q)

- 80:20 train–test split

- Model validation using MAPE

- Final model refit on full data to predict next month sales

📌 Purpose:

Generate short-term, region-specific sales forecasts.

# Forecasting Limitations 

- Small sample size increases risk of overfitting

- ARIMA models cannot capture:

  - Macro-economic shifts

  - Competitive actions

  - Sudden market shocks

- December 2018 outlier influences January 2019 forecasts

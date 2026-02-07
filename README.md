Stock Price Modeling Using AR & MA Models
Description

This project analyzes Apple (AAPL) stock prices using classical time series models, specifically Autoregressive (AR) and Moving Average (MA) models.

The objective is to model short-term stock return behavior, capture temporal dependencies in financial data, and evaluate model performance using statistical diagnostics such as AIC, BIC, and residual analysis.

The project demonstrates how AR and MA models can be applied to financial time series after transforming the data into a stationary form using log returns.

Installation

To run this notebook, install the following Python libraries:

pip install pandas numpy matplotlib statsmodels openpyxl

Usage
1️⃣ Data Loading and Preparation

Load cleaned stock data from an Excel file

Filter dataset for Apple (AAPL)

Sort by date and set Date as index

Extract the Close price series

2️⃣ Log Returns Calculation

Compute log returns from closing prices

Remove missing values

Prepare stationary time series

3️⃣ Stationarity Test

Perform the Augmented Dickey-Fuller (ADF) test

Confirm stationarity before modeling

4️⃣ ACF and PACF Plots

Generate ACF plot to identify MA(q) order

Generate PACF plot to identify AR(p) order

5️⃣ AR and MA Model Fitting

Fit AR(2) model

Fit MA(2) model

Use ARIMA framework for implementation

6️⃣ Model Evaluation

Compare models using AIC (Akaike Information Criterion)

Compare models using BIC (Bayesian Information Criterion)

Analyze residuals

Check residual autocorrelation

Model Evaluation Metrics

AIC – Lower value indicates better model fit

BIC – Penalizes model complexity

Residual diagnostics – Ensures residuals resemble white noise

Project Structure
├── cleaned_stock_details_5_years.xlsx
├── Stock_Price_Modeling.ipynb
└── README.md

Key Concepts Covered

Time Series Analysis

Stationarity

Log Returns

Autoregressive (AR) Model

Moving Average (MA) Model

Model Diagnostics

Contributing

Feel free to fork this repository, make improvements, and submit pull requests.

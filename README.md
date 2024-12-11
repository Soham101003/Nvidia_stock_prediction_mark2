# Nvidia Stock Price Prediction Project
In this project, I worked on predicting Nvidia’s stock prices in real-time using different time series forecasting and machine learning models. The goal was to analyze the stock’s historical data and predict its future prices with high accuracy. I leveraged ARIMA, Random Forest, and XGBoost for this task.

# Data Collection and Preprocessing
I used the yfinance library to collect historical stock data of Nvidia, including open, high, low, close prices, and volume. The data was preprocessed to handle missing values, outliers, and converted into a time series format for further analysis.
# Modeling approach
 implemented three different models to predict Nvidia stock prices:

# 1.ARIMA
 ARIMA (AutoRegressive Integrated Moving Average) ARIMA is a classical statistical model used for time series forecasting. It involves identifying patterns in the historical data, such as trend and seasonality, and making predictions based on these patterns.

Model Selection: The ARIMA model’s parameters (p, d, q) were selected using ACF and PACF plots.
## Performance Metrics for ARIMA:
Mean Squared Error (MSE): 17.21

Root Mean Squared Error (RMSE): 4.15

Mean Absolute Error (MAE): 3.76

R-squared (R²): -0.56 (indicating poor fit to data)

Mean Absolute Percentage Error (MAPE): 2.72%

Mean Absolute Scaled Error (MASE): 1.82

Normalized RMSE (%): 27.92%

Despite ARIMA’s potential, its performance wasn’t as robust due to the volatility in stock prices, which the model wasn’t fully equipped to handle.



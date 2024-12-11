Nvidia Stock Price Prediction Project
In this project, I worked on predicting Nvidia’s stock prices in real time using different time series forecasting and machine learning models. The goal was to analyze the stock’s historical data and predict its future prices with high accuracy. I leveraged ARIMA, Random Forest, and XGBoost for this task.

Data Collection and Preprocessing
I used the yfinance library to collect historical stock data of Nvidia, including open, high, low, close prices, and volume. The data was preprocessed to handle missing values, outliers, and converted into a time series format for further analysis.

Modeling Approach
I implemented three different models to predict Nvidia stock prices:

ARIMA (AutoRegressive Integrated Moving Average) ARIMA is a classical statistical model used for time series forecasting. It involves identifying patterns in the historical data, such as trend and seasonality, and making predictions based on these patterns.

Model Selection: The ARIMA model’s parameters (p, d, q) were selected using ACF and PACF plots.
Performance Metrics for ARIMA:
Mean Squared Error (MSE): 17.21
Root Mean Squared Error (RMSE): 4.15
Mean Absolute Error (MAE): 3.76
R-squared (R²): -0.56 (indicating poor fit to data)
Mean Absolute Percentage Error (MAPE): 2.72%
Mean Absolute Scaled Error (MASE): 1.82
Normalized RMSE (%): 27.92%
Despite ARIMA’s potential, its performance wasn’t as robust due to the volatility in stock prices, which the model wasn’t fully equipped to handle.

Random Forest Random Forest is an ensemble learning method that uses multiple decision trees to make predictions. It’s more flexible and handles non-linearity better than ARIMA.

Performance Metrics for Random Forest:
Mean Squared Error (MSE): 0.58
Root Mean Squared Error (RMSE): 0.76
Mean Absolute Error (MAE): 0.32
R² Score: 0.9994 (indicating an excellent fit)
Mean Absolute Percentage Error (MAPE): 1.87%
Mean Absolute Scaled Error (MASE): 1.11
The Random Forest model showed excellent results with a very high R² score, making it one of the best performing models for this task.

XGBoost XGBoost is a powerful gradient boosting algorithm that improves upon traditional decision trees by focusing on optimizing the model’s performance in a sequential manner. It also handles missing data and overfitting more effectively.

Performance Metrics for XGBoost:
Mean Squared Error (MSE): 1.75
Root Mean Squared Error (RMSE): 1.32
Mean Absolute Error (MAE): 0.49
R² Score: 0.9982
Mean Absolute Percentage Error (MAPE): 2.09%
Mean Absolute Scaled Error (MASE): 1.26
XGBoost showed strong performance with an R² score close to 1, similar to Random Forest, and outperformed ARIMA in terms of error metrics.

Real-time Application
To make the project more practical, I integrated yfinance to fetch real-time stock data, allowing the trained models to predict Nvidia’s stock price dynamically. The predictions could then be visualized in a dashboard for real-time tracking.

Conclusion
In this project, I compared multiple models for stock price prediction and found that Random Forest and XGBoost outperformed ARIMA by a significant margin, providing more accurate predictions with lower error metrics. The results from Random Forest and XGBoost were very promising, especially with their R² scores of 0.9994 and 0.9982, respectively.

For future improvements, I plan to incorporate sentiment analysis from news sources, social media, and other external factors that might impact stock prices. I also aim to explore deep learning approaches like LSTM (Long Short-Term Memory) networks for better handling of sequential data.

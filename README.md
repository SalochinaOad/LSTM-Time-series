# "DeepStock: LSTM-Based Time Series Forecasting for Stock Price Prediction"

### Problem Statement
Stock market prices are inherently sequential and volatile, making accurate prediction a complex task due to the influence of multiple dynamic factors. Traditional models often fall short in capturing the temporal dependencies within stock price data. This project aims to leverage the power of Recurrent Neural Networks, specifically Long Short-Term Memory (LSTM) networks, to predict the future opening price of Google stock based on historical data. By training the model on 60-day windows of past prices, we seek to capture short- and long-term trends in the data to improve forecasting accuracy and support data-driven financial decision-making.

- Architecture:

4 stacked LSTM layers (each with 50 units) to capture temporal dependencies

Dropout of 20% after each LSTM layer to prevent overfitting

A Dense layer with 1 unit to output the predicted price

- Compilation:

Optimizer: Adam

Loss function: Mean Squared Error (MSE) (suitable for regression tasks)

- Training:

Epochs: 100

Batch size: 32

Training samples: 1198 (after 60-timestep windowing)

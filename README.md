# deeplearningproj1
Stock Recommendation System Based on ESG Scores and LSTM Model
This repository contains a deep learning-based stock recommendation system, combining Environmental, Social, and Governance (ESG) scores with stock price predictions. The project leverages a Long Short-Term Memory (LSTM) model to predict stock price movements and integrates ESG scores to provide sustainable investment recommendations.

Project Overview:
The goal of this project is to create a stock recommendation system that not only predicts stock prices using historical data but also considers ESG scores to provide recommendations on environmentally sustainable companies. The system ranks companies by combining their predicted stock performance and ESG scores.

Key Hypotheses:
Companies with higher ESG scores tend to have more stable stock price growth over time. A deep learning model (LSTM) can predict stock performance based on historical stock data and ESG metrics. Investments in companies with higher ESG scores are likely to lead to better long-term financial returns.

Features:
LSTM Model: Uses historical stock price data to predict future stock prices.
ESG Integration: Merges ESG scores from a Kaggle dataset with stock data to assess company sustainability.
Stock Growth Comparison: Evaluates stock growth for companies with high vs. low ESG scores.
Investment Score Calculation: Creates a weighted investment score based on predicted stock performance and ESG scores.
Visualization: Graphical representations of real vs. predicted stock prices and top companies based on investment scores.

Data Sources:
Yahoo Finance: Stock data for various companies, fetched using the yfinance Python library.
ESG Dataset: ESG (Environmental, Social, Governance) scores for companies, sourced from Kaggle.

Model Architecture:
The project uses an LSTM (Long Short-Term Memory) neural network, a type of Recurrent Neural Network (RNN), to predict stock prices. The model is trained on multiple features, including stock prices (Open, High, Low, Close) and ESG scores (Environmental, Social, and Governance metrics).
Components of Architechture:
LSTM Layers: Used for time-series forecasting to predict stock price movements.
Dropout Layers: Applied to prevent overfitting during training.
Dense Layer: Outputs the predicted stock price.
MinMaxScaler: Used for feature scaling before training the model.

Usage
Data Fetching: The script fetches historical stock price data for a given set of companies using the yfinance API.
Data Preprocessing: The stock price data is normalized, and ESG scores are merged with the stock data.
LSTM Model Training: The LSTM model is trained on stock data to predict future stock prices.
Prediction: The model predicts future stock prices, and the results are combined with ESG scores to calculate investment recommendations.
Visualization: The system visualizes real vs. predicted stock prices and ranks companies based on their investment scores.

Results and Visualization
After training the model, the notebook provides the following insights:
- A comparison of real vs. predicted stock prices.
- The top 10 companies ranked by a combined investment score (predicted stock growth and ESG scores).
- Average stock growth across different ESG score quartiles to validate the hypothesis that high ESG scores correlate with stable stock performance.
Sample visualization:
![image](https://github.com/user-attachments/assets/6111c6cd-fcf0-499a-a856-93299b153cba)

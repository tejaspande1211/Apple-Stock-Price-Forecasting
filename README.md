# Apple Stock Price Forecasting using LSTM

## Overview
This project implements a time-series forecasting model to predict Apple Inc. (AAPL) stock closing prices using a Long Short-Term Memory (LSTM) neural network.  
The focus is on proper time-series preprocessing, avoiding data leakage, and evaluating short-horizon predictive performance.

## Dataset
- Historical daily stock price data for Apple Inc.
- Features used: Open, High, Low, Close, Volume
- Data sourced from publicly available financial APIs (e.g., Yahoo Finance)

## Methodology
- Chronological train-test split (no random shuffling)
- Feature scaling using Min-Max normalization (fit on training data only)
- Sliding window sequence generation for LSTM input
- LSTM-based regression model for price forecasting
- Evaluation using RMSE and MAE on the test set
- Separate visualization for evaluation and future forecasting

## Key Results
- The model captures short-term price trends reasonably well
- Prediction errors are quantified in price units using RMSE and MAE
- Clear separation between model evaluation and future forecasting avoids misinterpretation

## Limitations
- Stock prices are influenced by external events not captured in historical price data
- Long-term forecasts are unreliable due to market volatility
- This project is not intended as a trading strategy

## Repository Structure

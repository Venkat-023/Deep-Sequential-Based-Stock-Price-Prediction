Stock Price Prediction Using Deep Learning Models
Comparative Study of LSTM, GRU, Bi-LSTM, and Hybrid Architectures
Overview

This project focuses on predicting stock prices using advanced deep learning models designed for time-series forecasting. It presents a comparative analysis of four architectures:

Long Short-Term Memory (LSTM)
Gated Recurrent Unit (GRU)
Bidirectional LSTM (Bi-LSTM)
Hybrid LSTM-GRU Model

The study uses historical stock data from Tata Consultancy Services (TCS) and evaluates model performance using multiple statistical metrics.

Abstract

Stock price prediction is inherently challenging due to the volatile and non-linear nature of financial markets. This project implements and evaluates multiple deep learning models to forecast stock prices using historical data.

Experimental results demonstrate that the GRU model achieves the best performance, with the lowest prediction error (RMSE ≈ 42.50, MAE ≈ 30.66) and the highest R² score (0.9358), outperforming other architectures.

Objectives
Predict stock prices using deep learning models
Compare performance across multiple architectures
Analyze time-series forecasting effectiveness
Identify the most suitable model for financial prediction tasks
Dataset
Source: Historical stock data of Tata Consultancy Services (TCS)
Features:
Date
Open
High
Low
Close (primary target)
Volume
Key Notes:
Data is chronologically ordered
Closing price is used for prediction
Dataset spans multiple years for robust training
Methodology
1. Data Preprocessing
Handling missing values
Normalization using MinMaxScaler (0–1 range)
Sliding window approach with 60 time steps
Train-test split:
80% training
20% testing
2. Model Architectures
LSTM
Captures long-term dependencies
Uses memory cells and gating mechanisms
GRU
Simplified version of LSTM
Faster training with fewer parameters
Efficient for time-series learning
Bi-LSTM
Processes data in both forward and backward directions
Captures past and future context
Hybrid LSTM-GRU
Combines LSTM and GRU layers
Includes attention and normalization
Designed to leverage strengths of both models
3. Training Process
Models trained over multiple epochs
Loss optimization during training
Early stopping applied to prevent overfitting
Evaluation Metrics

The models are evaluated using the following metrics:

MAE (Mean Absolute Error)

MSE (Mean Squared Error)

RMSE (Root Mean Squared Error)

MAPE (Mean Absolute Percentage Error)

R² Score

Directional Accuracy

Results

Performance Comparison

Model	MAE	RMSE	R² Score	Accuracy

LSTM	69.56	92.23	0.78	48.5%

GRU	30.66	42.50	0.9358	99.06%

Bi-LSTM	—	—	—	54.3%

Hybrid LSTM-GRU	49.07	63.24	0.8618	98.5%


Key Observations

GRU performs best overall

Lowest error values

Highest R² score

Strong generalization

Hybrid model performs competitively

Better than standalone LSTM

Slightly below GRU

LSTM shows moderate performance

Struggles with short-term volatility

Bi-LSTM captures trends but lacks precision

Conclusion

GRU is the most effective model for stock price prediction in this study.

Hybrid LSTM-GRU offers strong alternative performance
LSTM and Bi-LSTM are less effective in capturing complex market patterns

Stock prediction remains difficult due to:

Market volatility

External influencing factors not captured in 

historical data

Future Work

Potential improvements include:

Incorporating news sentiment analysis

Adding macroeconomic indicators

Using real-time data streams

Exploring transformers and attention-based models

Enhancing feature engineering

Tech Stack

Python

TensorFlow / Keras

NumPy

Pandas

Scikit-learn

Matplotlib

# Stock-market-trend-prediction-using-dnn
Deep Neural Network–based stock price prediction using technical indicators, with a backtested trading strategy incorporating stop-loss and take-profit risk management.
# 📈 Stock Price Prediction Using Deep Neural Networks

This project implements an **end-to-end stock market prediction system** using **technical indicators** and a **Deep Neural Network (DNN)** to forecast next-day closing prices.  
Model predictions are converted into a **rule-based trading strategy** with **stop-loss and take-profit risk management**, and performance is evaluated against a **Buy-and-Hold benchmark**.

---

## 🚀 Project Features

- Historical stock data collection using Yahoo Finance  
- Technical indicator-based feature engineering  
- Deep Neural Network (DNN) for price prediction  
- Time-series aware train–test split (no data leakage)  
- Trading strategy based on model predictions  
- Stop-loss and take-profit risk management  
- Strategy performance comparison with Buy-and-Hold  

---

## 🧠 Technical Indicators Used

- Simple Moving Average (SMA)
- Exponential Moving Average (EMA)
- Relative Strength Index (RSI)
- MACD & Signal Line
- Bollinger Bands (Upper, Middle, Lower)
- Stochastic Oscillator (%K, %D)
- Average True Range (ATR)
- Previous Day Close (Lag Feature)

---

## 🏗️ Model Architecture

- **Input Layer**: Technical indicators  
- **Hidden Layers**: Dense layers with ReLU activation and Dropout  
- **Output Layer**: Single neuron predicting next-day closing price  
- **Loss Function**: Mean Squared Error (MSE)  
- **Optimizer**: Adam  

---

## 📊 Trading Strategy Logic

- **Buy**: Predicted price > Current close price  
- **Sell / Exit**:
  - Stop-loss triggered (2% downside)
  - Take-profit triggered (4% upside)
  - Model predicts price reversal  

The strategy is evaluated using portfolio value over time and compared against a Buy-and-Hold approach.

---

## 📈 Evaluation Metrics

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Strategy Return (%)
- Buy-and-Hold Return (%)

---

## 🛠️ Tech Stack

- Python  
- TensorFlow / Keras  
- pandas, numpy  
- yfinance  
- pandas-ta  
- scikit-learn  
- statsmodels  
- matplotlib  

---

## ▶️ How to Run the Project

1. Clone the repository  

git clone https://github.com/your-username/stock-price-prediction-dnn.git
cd stock-price-prediction-dnn

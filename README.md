
# 📊 Cryptocurrency Investment Analysis and Modelling using Machine Learning Algorithms

### 🔍 Project Overview

This project focuses on analyzing and predicting the prices of major cryptocurrencies using advanced machine learning (ML) and deep learning (DL) algorithms. Given the highly volatile nature of the crypto market, traditional statistical models often fall short in capturing the complex dynamics. This project presents a hybrid framework leveraging real-time data, technical indicators, and sequential models to improve forecasting accuracy.

---

## 🎯 Objectives

- Develop a predictive system for short-term cryptocurrency price forecasting (30-day horizon).
- Apply ML and DL models (Linear Regression, Random Forest, ARIMA, LSTM).
- Engineer features using financial technical indicators like SMA, EMA, RSI, and MACD.
- Evaluate models using MAE, RMSE, and R² score.
- Deploy the solution as a Django-based web application with real-time prediction capabilities using CoinGecko API.

---

## 💡 Key Research Questions

1. How effective are LSTM models vs traditional ML models in volatile crypto markets?
2. What role do technical indicators play in improving prediction accuracy?
3. How does preprocessing impact the performance of forecasting models?
4. Can market sentiment and trend-based indicators be integrated effectively?
5. How reliable is the proposed model across different market conditions?

---

## 📁 Dataset Summary

### 📌 Sources:
- [Yahoo Finance](https://finance.yahoo.com)
- [CoinGecko API](https://coingecko.com)
- FirstRateData for minute-wise price data

### 📊 Datasets Used:
- **Minute-wise Bitcoin price data** (2024-07-07 to 2024-07-22): 22,799 records
- **Day-wise Bitcoin price data** (2018-2023): 1,827 records
- **Five Cryptocurrencies**: BTC, ETH, XMR, XRP, BCH

### 🔑 Features:
- Date, Open, High, Low, Close, Adjusted Close, Volume
- Derived Features: SMA, EMA, RSI, MACD

---

## ⚙️ Methodology

### 🔧 Data Preprocessing
- Handled missing values using forward fill and interpolation.
- Removed outliers using Z-score and IQR methods.
- Feature scaling using Min-Max Normalization to bring all features in range [0, 1].

### 🧠 Feature Engineering
- **SMA/EMA** to capture trend direction
- **RSI** to identify overbought/oversold conditions
- **MACD** to detect momentum shifts and divergence signals
- **Time-series decomposition** to analyze trend, seasonality, and residuals

### 📈 Models Implemented
- **Machine Learning**: Linear Regression, Random Forest, ARIMA
- **Deep Learning**: Long Short-Term Memory (LSTM)

---

## 🧪 Experimental Setup

### 💻 Hardware
- Intel i7-12700K, 32GB RAM, 1TB SSD, NVIDIA RTX 3090

### 🧰 Software Stack
- Python 3.8, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow, Keras, TA-Lib, Django, CoinGecko API

---

## 🧾 Results & Evaluation

| Model             | RMSE       | MAE        | R² Score |
|------------------|------------|------------|----------|
| Linear Regression| Moderate   | Moderate   | ~0.75    |
| Random Forest     | Good       | Good       | ~0.85    |
| ARIMA             | Poor       | Poor       | <0.70    |
| **LSTM**          | **Excellent** | **Excellent** | **Up to 0.97 (BTC)** |

✅ LSTM outperformed all other models, particularly in medium to short-term forecasts.

✅ Random Forest performed best on Monero (XMR).

---

## 🌐 Web Application

A Django-based web app integrates real-time price data using CoinGecko API. It allows:
- Input of selected cryptocurrency
- Visualization of past 30 days' prices
- Forecast of next 30 days’ trends using trained models
- User-friendly interface for traders and investors

---

## 🧭 Future Work

- Integrate sentiment analysis from Twitter and Reddit
- Include on-chain metrics and macroeconomic indicators
- Implement GRU and Transformer models for comparison
- Enable user authentication and portfolio tracking in web app

---

## 📚 References

- [FreeCodeCamp – Regression Metrics](https://www.freecodecamp.org/news/evaluation-metrics-for-regression-problems-machine-learning/)
- [Machine Learning Mastery – Regression Models](https://machinelearningmastery.com/regression-metrics-for-machine-learning/)
- [Crypto.com Price Tracker](https://crypto.com/price)
- [Forbes Digital Assets](https://www.forbes.com/digital-assets)
- [GeeksforGeeks – Python ML Libraries](https://www.geeksforgeeks.org/best-python-libraries-for-machine-learning/)

---

## 👤 Author

Rohit Satish Jyotibannad
Student ID: H00461485  
Email: [rs2156@hw.ac.uk](mailto:rs2156@hw.ac.uk)  
Supervised by: Prof. Jurriaan Hage  
School of Mathematics and Computer Science  
Heriot-Watt University

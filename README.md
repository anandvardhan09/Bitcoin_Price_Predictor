# 📈 Bitcoin Price Prediction with LSTM, ARIMA, and XGBoost

This project focuses on building a robust pipeline for forecasting Bitcoin prices using a hybrid approach — combining deep learning (LSTM), traditional statistical modeling (ARIMA), and ensemble machine learning (XGBoost). We leverage walk-forward validation, technical indicators, and multiple metrics to evaluate performance and model reliability.

---

## 🚀 Overview

- **Goal**: Predict future Bitcoin closing prices using historical data and engineered technical features.
- **Data Source**: [Yahoo Finance](https://finance.yahoo.com/)
- **Models Used**: 
  - Long Short-Term Memory (LSTM)
  - ARIMA
  - XGBoost Regressor

---

## 🛠️ Features Engineered

- **Returns**: Daily % change in closing price
- **MA7, MA30**: 7-day and 30-day moving averages
- **Volatility**: Rolling standard deviation over 7 days
- **RSI**: 14-day Relative Strength Index (momentum indicator)

---

## 🔁 Walk-Forward Validation

To mimic real-world forecasting conditions, walk-forward validation was implemented. The model is retrained and tested on sliding time windows to simulate production-like performance without future leakage.

---

## 📊 Model Evaluation Metrics

- **MSE (Mean Squared Error)**
- **RMSE (Root Mean Squared Error)**
- **MAE (Mean Absolute Error)**
- **R² Score**
- **Improvement over Naive Baseline (%)**

---


## 📌 Key Insights

- Feature engineering added valuable signals but high volatility limited model generalization.
- LSTM performed slightly better than XGBoost and significantly better than ARIMA.
- XGBoost provided feature importance insights for interpretability.
- ARIMA struggled due to non-stationarity and lack of engineered features.

---

## 🧠 Future Improvements

- Use **hyperparameter tuning** (GridSearchCV / KerasTuner)
- Explore **Transformer-based** time series models
- Add more **technical indicators** (MACD, Bollinger Bands)
- Integrate **backtesting** for strategy simulation
- Package results in a **Streamlit dashboard** or REST API

---


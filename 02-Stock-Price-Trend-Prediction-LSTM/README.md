# 📈 Stock Price Trend Prediction using Stacked LSTM

An end-to-end deep learning pipeline to forecast equity price trends using a 2-layer Stacked Long Short-Term Memory (LSTM) recurrent neural network with Dropout regularization, deployed to Streamlit Cloud.

---

## 🚀 Live Demo & Artifacts
* **Streamlit Web Application:** [Live Forecasting Dashboard](https://kqz4ge4a9o4.streamlit.app)
* **Dataset:** Yahoo Finance Historical Market Data (AAPL, 2015–2024)

---

## 🛠️ System Architecture & Workflow
1. **Data Ingestion & Technical Indicators:**
   * Historical daily records retrieved via `yfinance`.
   * Extracted 50-day SMA, 200-day SMA, and 14-day Relative Strength Index (RSI).
2. **Tensor Preprocessing:**
   * Scaled using `MinMaxScaler` $[0, 1]$.
   * Restructured into 60-day lookback sequences formatted as 3D tensors: `(samples, 60, 1)`.
   * Partitioned into chronological 80% train and 20% test splits.
3. **Stacked LSTM Architecture:**
   * LSTM (50 units, `return_sequences=True`) + Dropout (0.2)
   * LSTM (50 units, `return_sequences=False`) + Dropout (0.2)
   * Dense (25 units) $\rightarrow$ Dense (1 unit)
   * Optimizer: Adam | Loss: Mean Squared Error (MSE)
4. **Interactive UI:**
   * Streamlit dashboard providing dynamic stock lookup, technical indicator plots, and on-demand model inference.

---

## 📊 Performance Metrics
* **Root Mean Squared Error (RMSE):** 2.51 USD
* **Mean Absolute Error (MAE):** 1.98 USD
* **Validation Loss:** 0.0031

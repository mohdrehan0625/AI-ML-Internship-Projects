# 🚀 AI/ML Internship Projects

This repository consolidates the complete end-to-end deliverables for the AI/ML internship projects, featuring data preprocessing pipelines, exploratory analysis, model training notebooks, performance benchmarks, and production-ready cloud web applications[span_0](start_span)[span_0](end_span)[span_1](start_span)[span_1](end_span)[span_2](start_span)[span_2](end_span).

---

## 📂 Projects Directory

### 1. [Credit Card Fraud Detection System](./01-Credit-Card-Fraud-Detection/)
* **Domain:** Machine Learning & Anomaly Detection[span_3](start_span)[span_3](end_span)[span_4](start_span)[span_4](end_span)
* **Description:** An end-to-end machine learning system engineered to detect fraudulent credit card transactions from highly skewed tabular data using unsupervised anomaly detection, supervised gradient boosting, and an interactive scoring dashboard[span_5](start_span)[span_5](end_span)[span_6](start_span)[span_6](end_span).
* **Tech Stack:** Python, Scikit-Learn, XGBoost, Imbalanced-Learn, Pandas, NumPy, Streamlit[span_7](start_span)[span_7](end_span)[span_8](start_span)[span_8](end_span)
* **Key Techniques:** Outlier-resilient scaling (`RobustScaler`), SMOTE balancing, Isolation Forest, Local Outlier Factor (LOF), and XGBoost Classifier[span_9](start_span)[span_9](end_span)[span_10](start_span)[span_10](end_span).
* **Live Web App:** [Credit Card Fraud Detector](https://credit-card-fraud-detection-juzs2.streamlit.app)[span_11](start_span)[span_11](end_span)

---

### 2. [Stock Price Trend Prediction with Stacked LSTM](./02-Stock-Price-Trend-Prediction-LSTM/)
* **Domain:** Deep Learning & Financial Time-Series Forecasting[span_12](start_span)[span_12](end_span)[span_13](start_span)[span_13](end_span)
* **Description:** A sequential deep learning forecasting engine designed to predict equity price momentum using a 2-layer Stacked Long Short-Term Memory (LSTM) recurrent neural network regularized with Dropout[span_14](start_span)[span_14](end_span)[span_15](start_span)[span_15](end_span).
* **Tech Stack:** Python, TensorFlow / Keras, Yahoo Finance API (`yfinance`), Pandas, NumPy, Matplotlib, Streamlit[span_16](start_span)[span_16](end_span)[span_17](start_span)[span_17](end_span)
* **Key Architecture & Pipeline:** 60-day sliding window sequences, `MinMaxScaler` normalization, 50/200-day Simple Moving Averages (SMA), 14-day Relative Strength Index (RSI), and dual-layer LSTM network[span_18](start_span)[span_18](end_span)[span_19](start_span)[span_19](end_span).
* **Evaluation Metrics:** RMSE: **2.51 USD** | MAE: **1.98 USD** | Final Validation Loss: **0.0031**[span_20](start_span)[span_20](end_span)
* **Live Web App:** [Stock Trend Dashboard](https://kqz4ge4a9o4.streamlit.app)[span_21](start_span)[span_21](end_span)[span_22](start_span)[span_22](end_span)

---

## 💻 Local Setup & Execution

Clone this repository and launch either application locally:

```bash
# Clone the repository
git clone [https://github.com/mohdrehan0625/AI-ML-Internship-Projects.git](https://github.com/mohdrehan0625/AI-ML-Internship-Projects.git)
cd AI-ML-Internship-Projects

# Run Project 1 (Credit Card Fraud Detection)
cd 01-Credit-Card-Fraud-Detection
pip install -r requirements.txt
streamlit run app.py

# Or Run Project 2 (Stock Price Trend Prediction)
cd ../02-Stock-Price-Trend-Prediction-LSTM
pip install -r requirements.txt
streamlit run app.py

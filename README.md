# 🚀 AI/ML Internship Projects

This repository consolidates the complete end-to-end deliverables for the AI/ML internship projects, featuring data preprocessing pipelines, exploratory analysis, model training notebooks, performance benchmarks, and production-ready cloud web applications.

---

## 📂 Projects Directory

### 1. [Credit Card Fraud Detection System](./01-Credit-Card-Fraud-Detection/)
* **Domain:** Machine Learning & Anomaly Detection
* **Description:** An end-to-end machine learning system engineered to detect fraudulent credit card transactions from highly skewed tabular data using unsupervised anomaly detection, supervised gradient boosting, and an interactive scoring dashboard.
* **Tech Stack:** Python, Scikit-Learn, XGBoost, Imbalanced-Learn, Pandas, NumPy, Streamlit
* **Key Techniques:** Outlier-resilient scaling (`RobustScaler`), SMOTE balancing, Isolation Forest, Local Outlier Factor (LOF), and XGBoost Classifier.
* **Live Web App:** [Credit Card Fraud Detector](https://credit-card-fraud-detection-juzs2.streamlit.app)

---

### 2. [Stock Price Trend Prediction with Stacked LSTM](./02-Stock-Price-Trend-Prediction-LSTM/)
* **Domain:** Deep Learning & Financial Time-Series Forecasting
* **Description:** A sequential deep learning forecasting engine designed to predict equity price momentum using a 2-layer Stacked Long Short-Term Memory (LSTM) recurrent neural network regularized with Dropout.
* **Tech Stack:** Python, TensorFlow / Keras, Yahoo Finance API (`yfinance`), Pandas, NumPy, Matplotlib, Streamlit
* **Key Architecture & Pipeline:** 60-day sliding window sequences, `MinMaxScaler` normalization, 50/200-day Simple Moving Averages (SMA), 14-day Relative Strength Index (RSI), and dual-layer LSTM network.
* **Evaluation Metrics:** RMSE: **2.51 USD** | MAE: **1.98 USD** | Final Validation Loss: **0.0031**
* **Live Web App:** [Stock Trend Dashboard](https://kqz4ge4a9o4.streamlit.app)

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

# 📈 StockPredict AI: Reliance Stock Price Prediction

[![Python 3.12+](https://img.shields.io/badge/python-3.12+-blue.svg)](https://www.python.org/downloads/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15+-FF6F00?logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Predicting Reliance Industries stock prices using Deep Learning (Bidirectional LSTM) with high precision.**

StockPredict AI is a sophisticated deep learning project designed to forecast the stock price of Reliance Industries (NSE: RELIANCE). By leveraging Bidirectional Long Short-Term Memory (LSTM) networks, the model captures complex temporal dependencies and market patterns that traditional machine learning models often miss.

---

## 🏆 Model Performance

The Bidirectional LSTM model significantly outperforms standard regression baselines, achieving near-perfect tracking of stock trends.

| Metric | Value |
| :--- | :--- |
| **R² Score** | **0.9682** ⭐ |
| **MAPE (Mean Absolute % Error)** | **1.63%** |
| **RMSE (Root Mean Square Error)** | **₹27.00** |
| **MAE (Mean Absolute Error)** | **₹21.34** |

---

## 📊 Dataset Information

The model is trained on historical data for **Reliance Industries Limited (RELIANCE.NS)**, one of India's largest conglomerates.

- **Source:** Yahoo Finance (via `yfinance` API)
- **Time Period:** 10 Years (January 1, 2015 – December 31, 2024)
- **Data Points:** 2,460+ trading sessions
- **Features Extracted:**
  - `Close`: Daily closing price
  - `High/Low`: Daily price range
  - `Volume`: Trading activity
  - `MA_20 / MA_50`: Moving averages for trend detection
  - `Volatility`: 20-day rolling standard deviation of returns

---

## 🧠 Project Architecture

The project follows a rigorous data science pipeline:

### 1. Data Collection & Preprocessing
Automated ingestion of NSE data, scaling using `MinMaxScaler`, and sequence generation (60-day windows).

### 2. Exploratory Data Analysis (EDA)
Comprehensive visualization of price trends, volatility analysis, and feature correlation studies.

### 3. Baseline Comparison
Evaluation of traditional models to establish a performance floor:
- **Logistic Regression**: 51.67% accuracy (direction)
- **Random Forest**: 48.75% accuracy (direction)
- **Gradient Boosting**: 49.16% accuracy (direction)

### 4. Deep Learning Model (Bidirectional LSTM)
A robust architecture featuring:
- Two Bidirectional LSTM layers for forward and backward temporal context.
- Dropout regularization to prevent overfitting.
- Adam optimizer with dynamic learning rate reduction.

### 5. Future Forecasting
Predicting price trends for the next 30 days with confidence intervals.

---

## 🚀 Tech Stack

- **Deep Learning:** TensorFlow, Keras
- **Machine Learning:** Scikit-learn
- **Data Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Financial Data:** YFinance (Yahoo Finance NSE)

---

## ⚡ Installation & Usage

### 1. Clone the Repository
```bash
git clone https://github.com/bytecraft17/StockPredict-AI.git
cd StockPredict-AI
```

### 2. Install Dependencies
```bash
pip install yfinance tensorflow scikit-learn pandas numpy matplotlib seaborn
```

### 3. Run the Notebook
```bash
jupyter notebook StockPredict_AI.ipynb
```

---

## 👤 Author

**bytecraft17**  
*AI/ML Developer*  
[GitHub Profile](https://github.com/bytecraft17)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
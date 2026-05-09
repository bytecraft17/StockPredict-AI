# 📈 StockPredict AI

> Reliance Industries Stock Price Prediction using Bidirectional LSTM | R²: 0.9682 | MAPE: 1.63%

---

## 🏆 Results

| Metric | Value |
|--------|-------|
| R² Score | **0.9682** ⭐ |
| MAPE | **1.63%** |
| RMSE | ₹27.00 |
| MAE | ₹21.34 |

---

## 📊 Model Comparison

| Model | Result |
|-------|--------|
| Logistic Regression | 51.67% accuracy |
| Random Forest | 48.75% accuracy |
| Gradient Boosting | 49.16% accuracy |
| **Bidirectional LSTM** ⭐ | **R²: 0.9682 — MAPE: 1.63%** |

> Basic ML fails at stock prediction — LSTM captures temporal patterns effectively.

---

## 🧠 Project Modules

### Module 1 — Data Collection
- Reliance Industries (RELIANCE.NS) — NSE India
- 10 years data: 2015-2024
- Source: Yahoo Finance via `yfinance`
- 2,400+ trading days

### Module 2 — EDA & Feature Engineering
- Closing price trend analysis
- Moving Averages (MA20, MA50)
- RSI — Relative Strength Index
- MACD + Signal Line
- Bollinger Bands
- Daily Returns & Volatility

### Module 3 — Basic ML (Baseline)
- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier
- Result: ~50% accuracy (coin flip) — proves stock direction prediction is hard

### Module 4 — Bidirectional LSTM
- 60-day sequences → Next day price
- 2 Bidirectional LSTM layers
- Dropout regularization
- EarlyStopping + ReduceLROnPlateau
- **Final R²: 0.9682 | MAPE: 1.63%** ⭐

### Module 5 — Future Forecast
- 30-day future price prediction
- Confidence band visualization

---

## 🏗️ Project Structure

---

## 🚀 Tech Stack

- **Deep Learning:** TensorFlow, Keras — Bidirectional LSTM
- **ML Models:** Scikit-learn
- **Data:** yfinance (Yahoo Finance NSE)
- **Visualization:** Matplotlib, Seaborn
- **Stock:** Reliance Industries (RELIANCE.NS)

---

## ⚡ How to Run

```bash
# 1. Clone the repo
git clone https://github.com/bytecraft17/StockPredict-AI.git

# 2. Install dependencies
pip install yfinance tensorflow scikit-learn pandas numpy matplotlib seaborn

# 3. Open notebook
jupyter notebook StockPredict_AI.ipynb

# 4. Run all cells
```

> Dataset downloads automatically via yfinance — no manual download needed!

---

## 👤 Author

**bytecraft17** — AI/ML Developer
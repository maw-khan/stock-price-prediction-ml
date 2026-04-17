# 📈 Stock Price Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)
![Dataset](https://img.shields.io/badge/Dataset-YFinance-purple)
![Type](https://img.shields.io/badge/Type-Time--Series-red)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 📌 Project Overview

This project focuses on predicting short-term stock prices using historical market data of Tesla (TSLA). It applies machine learning techniques along with feature engineering and time-series aware validation to model stock behavior.

The goal is not to "perfectly predict the market", but to analyze how well machine learning models can capture short-term trends in financial data.

---

## 🎯 Objectives

- Build a machine learning pipeline for stock prediction
- Engineer meaningful time-series features
- Avoid data leakage using chronological splitting
- Compare Linear Regression and Random Forest models
- Evaluate model performance using regression metrics
- Interpret feature importance and residual behavior

---

## 📊 Dataset

- Source: Yahoo Finance (via `yfinance`)
- Stock: Tesla (TSLA)
- Time Period: 2018 – 2024
- Features: Open, High, Low, Close, Volume

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Handled missing values
- Flattened dataset structure
- Sorted data chronologically

### 2. Feature Engineering
- Lag features (1, 2, 3 days)
- Rolling mean (5-day, 10-day)
- Rolling standard deviation

### 3. Modeling
- Linear Regression (baseline model)
- Random Forest Regressor (non-linear model)

### 4. Evaluation
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score

---

## 📈 Results

| Model | MAE | RMSE | R² Score |
|------|-----|------|----------|
| Linear Regression | 6.42 | 9.30 | 0.97 |
| Random Forest | 8.64 | 15.18 | 0.93 |

---

## 🧠 Key Insights

- Stock prices show strong short-term autocorrelation
- Recent price values are the most important predictors
- Engineered features improve interpretability but not always dominance
- Models perform better in stable markets than volatile periods

---

## 📉 Visualizations

- Actual vs Predicted Prices
- Feature Importance Analysis
- Residual Error Distribution

---

## ⚠️ Limitations

- Does not include external factors (news, sentiment, macroeconomics)
- Not suitable as a real trading strategy
- Performance may vary under extreme market conditions

---

## 🚀 Future Work

- LSTM / Transformer-based models
- Sentiment analysis integration
- Macro-economic feature inclusion
- Multi-stock portfolio modeling

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- yFinance

---

## 📌 Author

Muhammad Ali Waris Khan

# 📈 Apple Stock Trend Prodiction

This project downloads historical stock data for Apple Inc. (AAPL) using Yahoo Finance, performs feature engineering, trains a Random Forest classifier to predict the direction of the next day's price, and visualizes stock trends and correlations.

---

## Project Overview

The notebook performs the following:

1. **Downloads Apple stock data** from January 1, 2020 to December 31, 2024.
2. **Plots the closing price** to visualize overall trends.
3. **Engineers features** such as:
   - Moving averages (MA5, MA10)
   - Volatility
   - Tomorrow’s price and binary target (price goes up or not)
4. **Trains a Random Forest model** to predict the stock price movement.
5. **Evaluates model performance** using classification metrics.
6. **Visualizes feature correlations** using a heatmap.

---

## Dependencies

Make sure you have the following Python libraries installed:

pip install yfinance matplotlib seaborn scikit-learn pandas

## Model Used
The model used for this project is the **Random Forest Classifier** from **scikit-learn**.

### Key Features:
- **Predicts**: Whether the next day's price will be higher than today's price based on historical stock data and engineered features.
- **Algorithm**: Random Forest Classifier




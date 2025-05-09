# 📈 Apple Stock Trend Projection

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


## Outputs

**Price Plot**: 
Line graph of AAPL closing price.

![Price Plot](https://github.com/user-attachments/assets/1e16f0e4-f786-4376-97dc-3e75908a3704)

**Feature Engineering**:
1. Tomorrow’s price
2. Moving averages (MA5 and MA10)
3. Volatility

The dataset contains the following stock price data for **Apple (AAPL)** from 2020-01-01 to 2024-12-31:

| Date       | Price | Close    | High    | Low     | Open    | Volume    | Tomorrow | Target | MA5      | MA10     | Volatility |
|------------|-------|----------|---------|---------|---------|-----------|----------|--------|----------|----------|------------|
| 2020-01-15 | 75.38 | 76.38    | 74.94   | 75.50   | 121923600 | 76.32    | 1        | 75.58    | 74.09    | 1.68       | 1.682775  |
| 2020-01-16 | 76.32 | 76.43    | 75.56   | 75.92   | 108829200 | 77.17    | 1        | 75.85    | 74.45    | 1.74       | 1.741704  |
| 2020-01-17 | 77.17 | 77.17    | 76.26   | 76.57   | 137816400 | 76.64    | 0        | 76.26    | 74.96    | 1.70       | 1.702722  |
| 2020-01-21 | 76.64 | 77.24    | 76.50   | 76.79   | 110843200 | 76.92    | 1        | 76.24    | 75.37    | 1.55       | 1.549409  |
| 2020-01-22 | 76.92 | 77.47    | 76.82   | 77.13   | 101832400 | 77.29    | 1        | 76.48    | 75.83    | 1.16       | 1.156558  |

**Classification Report**:

The model's classification performance:

| Metric         | Precision | Recall  | F1-Score | Support |
|----------------|-----------|---------|----------|---------|
| **0**          | 0.43      | 0.84    | 0.57     | 108     |
| **1**          | 0.57      | 0.16    | 0.25     | 142     |
| **Accuracy**   | -         | -       | 0.46     | 250     |
| **Macro avg**  | 0.50      | 0.50    | 0.41     | 250     |
| **Weighted avg**| 0.51     | 0.46    | 0.39     | 250     |

**Heatmap**: Correlation between engineered features.

![Heatmap](https://github.com/user-attachments/assets/ea8f922d-1a82-4e80-ac37-c5a8f21cb7b0)

## Model Used
The model used for this project is the **Random Forest Classifier** from **scikit-learn**.

### Key Features:
- **Predicts**: Whether the next day's price will be higher than today's price based on historical stock data and engineered features.
- **Algorithm**: Random Forest Classifier




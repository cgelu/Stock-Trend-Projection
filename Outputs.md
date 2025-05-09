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

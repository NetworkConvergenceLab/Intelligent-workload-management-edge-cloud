# Paired Bootstrap Significance Tests

XGBoost = baseline; n=10,000 bootstrap resamples.  
* indicates p<0.05. ↑ = XGBoost performs better, ↓ = XGBoost performs worse.

## Cloud CPU (5-min)

| Comparison | F1 p-value | R² p-value | RMSE p-value |
|------------|-----------|-----------|-------------|
| vs ARIMAX  | 0.012* ↑  | 0.000* ↑  | 0.000* ↑    |
| vs LSTM    | 0.000* ↑  | 0.001* ↑  | 0.000* ↑    |
| vs DLinear | 0.000* ↓  | 0.260 ↓   | 0.611 ↓     |
| vs TFT     | 0.596 ↑   | 0.061 ↑   | 0.059 ↑     |

## Cloud Memory (5-min)

| Comparison | F1 p-value | R² p-value | RMSE p-value |
|------------|-----------|-----------|-------------|
| vs ARIMAX  | 0.000* ↑  | 0.000* ↑  | 0.000* ↑    |
| vs LSTM    | 0.000* ↑  | 0.302 ↑   | 0.279 ↑     |
| vs DLinear | 0.000* ↑  | 0.000* ↓  | 0.000* ↓    |
| vs TFT     | 0.099 ↑   | 0.320 ↑   | 0.304 ↑     |

## Edge CPU — τ-max-in-T (5-minute-max-in-40)

| Comparison | F1 p-value | R² p-value | RMSE p-value |
|------------|-----------|-----------|-------------|
| vs ARIMAX  | 0.000* ↓  | 0.000* ↑  | 0.000* ↑    |
| vs LSTM    | 0.000* ↑  | 0.011* ↓  | 0.008* ↓    |
| vs DLinear | 0.000* ↑  | 0.000* ↓  | 0.000* ↓    |
| vs TFT     | 0.000* ↑  | 0.140 ↑   | 0.132 ↑     |

## Edge Memory — τ-max-in-T (5-minute-max-in-40)

| Comparison | F1 p-value | R² p-value | RMSE p-value |
|------------|-----------|-----------|-------------|
| vs ARIMAX  | 0.000* ↑  | 0.028* ↑  | 0.000* ↓    |
| vs LSTM    | 0.000* ↑  | 0.000* ↑  | 0.000* ↑    |
| vs DLinear | 0.000* ↑  | 0.000* ↑  | 0.000* ↑    |
| vs TFT     | 0.033* ↑  | 0.000* ↑  | 0.000* ↑    |

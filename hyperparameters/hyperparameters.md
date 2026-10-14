# Section V-A: Hyperparameters

Bayesian optimisation was used for all models on a 20% hold-out validation subset of the training data.

## Cloud (5-min)

| Algorithm | CPU | Memory |
|-----------|-----|--------|
| ARIMAX | p,d,q: (11,0,5) | p,d,q: (3,0,2) |
| LSTM | Units1: 190, Units2: 84, Dropout: 0.4924, LR: 0.00113, Batch: 93 | Units1: 152, Units2: 156, Dropout: 0.3489, LR: 0.00475, Batch: 32 |
| XGBoost | Estimators: 291, Max Depth: 3, LR: 0.074349 | Estimators: 331, Max Depth: 4, LR: 0.0159 |
| DLinear | Kernel: 10, LR: 0.00077, Batch: 32 | Kernel: 10, LR: 0.00077, Batch: 32 |
| TFT | Hidden: 32, Heads: 4, FF: 64, Dropout: 0.10, LR: 0.001, Batch: 64 | Hidden: 32, Heads: 4, FF: 64, Dropout: 0.10, LR: 0.001, Batch: 64 |

## Edge DC (5-min)

| Algorithm | CPU | Memory |
|-----------|-----|--------|
| ARIMAX | p,d,q: (8,0,4) | p,d,q: (12,0,0) |
| LSTM | Units1: 48, Units2: 105, Dropout: 0.233, LR: 0.00017, Batch: 94 | Units1: 38, Units2: 136, Dropout: 0.100, LR: 0.00411, Batch: 94 |
| XGBoost | Estimators: 400, Max Depth: 3, LR: 0.010 | Estimators: 400, Max Depth: 3, LR: 0.010 |
| DLinear | Kernel: 11, LR: 0.00013, Batch: 128 | Kernel: 10, LR: 0.00167, Batch: 32 |
| TFT | Hidden: 32, Heads: 4, FF: 64, Dropout: 0.10, LR: 0.001, Batch: 64 | Hidden: 32, Heads: 4, FF: 64, Dropout: 0.10, LR: 0.001, Batch: 64 |

## Edge DC (5-minute-max-in-40)

| Algorithm | CPU | Memory |
|-----------|-----|--------|
| ARIMAX | p,d,q: (2,0,4) | p,d,q: (13,0,4) |
| LSTM | Units1: 41, Units2: 148, Dropout: 0.47542, LR: 0.0001, Batch: 127 | Units1: 77, Units2: 132, Dropout: 0.41237, LR: 0.00022, Batch: 32 |
| XGBoost | Estimators: 400, Max Depth: 6, LR: 0.01 | Estimators: 138, Max Depth: 6, LR: 0.0385 |
| DLinear | Kernel: 15, LR: 0.00125, Batch: 128 | Kernel: 9, LR: 0.00046, Batch: 32 |
| TFT | Hidden: 32, Heads: 4, FF: 64, Dropout: 0.10, LR: 0.001, Batch: 64 | Hidden: 32, Heads: 4, FF: 64, Dropout: 0.10, LR: 0.001, Batch: 64 |

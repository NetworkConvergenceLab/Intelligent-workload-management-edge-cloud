# Section VI-C: Memory Performance Results

Detailed evaluation metrics for memory prediction across cloud and edge DC settings.
Corresponds to Figures 2d, 2e, and 2f in the paper.

---

## Cloud-Scale Memory Prediction (Figure 2d)

RMSE ranges from 153.72 to 165.59, MAE ranges from 100.06 to 116.85, and MAPE ranges from 2.62 to 3.02, with R² in [0.83–0.86]. DLinear achieves the lowest RMSE (153.72), MAE (100.06), and MAPE (2.62), as well as the highest R² of 0.86. This is driven by the difference in resource scale between CPU and Memory, whereby CPU capacity is in the order of 28×10³ as opposed to Memory 5×10³.

---

## Edge-Scale Memory Prediction — 5-minute (Figure 2e)

RMSE ranges from 0.041 to 0.042, MAE is approximately 0.032, and MAPE ranges from 38.32% to 41.29%, with R² ranging from 0.216 to 0.253.

---

## Edge-Scale Memory Prediction — 5-minute-max-in-40 (Figure 2f)

Performance improves more consistently, with R² increasing to 0.373–0.407, MAPE decreasing to 19.85%–20.65%, and RMSE and MAE decreasing marginally to 0.038–0.039 and 0.029–0.030, respectively. XGBoost achieves the highest R² (0.407), while ARIMAX achieves the lowest MAPE (19.85%).

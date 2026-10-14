
# Section IV-B: Benchmarked Algortihms

## ARIMAX
ARIMAX extends ARIMA by incorporating exogenous variables into the forecasting process, allowing the model to exploit information beyond the historical target series. ARIMAX retains the (p,d,q) structure but additionally includes explanatory variables that may influence future resource demand. In this work, these exogenous inputs consist of engineered workload features and temporal features (hour-of-day and day-of-week). By incorporating additional workload context, ARIMAX can capture relationships that are not represented by the autoregressive component alone, making it well suited for workload forecasting applications.

## Decomposition Linear Model (DLinear)
DLinear is a lightweight time series forecasting model that decomposes the input sequence into trend and seasonal components using a moving average filter, then applies separate linear layers to each component. Despite its simplicity, DLinear has been shown to outperform complex Transformer-based architectures on standard long-term forecasting benchmarks, demonstrating that linear models can effectively capture temporal patterns in smooth, autocorrelated workloads. In this work, DLinear is applied in its univariate formulation, using only the target series history as input, consistent with its channel-independence design principle.

## Extreme Gradient Boosting (XGBoost)
XGBoost is a gradient-boosting algorithm well suited to structured, feature-rich datasets. It iteratively builds an ensemble of decision trees, each correcting errors from previous trees. Unlike conventional time-series models, it relies on engineered features, such as lagged values and rolling statistics, rather than explicitly modelling temporal dependencies.

## Long Short-Term Memory (LSTM)
LSTM is a recurrent neural network (RNN) designed to capture long-term dependencies in sequential data. Its memory cells and gates enable it to learn trends and seasonality without explicitly specifying lag structures. However, its complex architecture may limit its ability to capture sharp peaks, favoring gradual trend prediction.

## Temporal Fusion Transformer (TFT)
The Transformer-based model implemented in this work incorporates key architectural components from the Temporal Fusion Transformer (TFT), including Gated Residual Networks (GRN), variable selection via softmax gating, and multi-head self-attention. The architecture is adapted for single-step peak-aware forecasting, omitting static covariate encoders and multi-horizon outputs not applicable in this work.

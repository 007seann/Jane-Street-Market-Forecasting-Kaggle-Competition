**Jane Street Real-Time Market Forecasting (24M-row dataset), Kaggle Competition**

- Conducted **EDA and time-series analysis** on anonymised financial data: analysed feature–feature and feature–responder correlations, identified non-stationarity, missing values, and fat-tailed distributions; designed preprocessing pipeline with **median imputation, robust scaling, and winsorization**.
- Benchmarked models under identical preprocessing:
    - **Ridge regression** (R² ≈ 0.003) — stable but underfit, captured weak linear structure only.
    - **XGBoost** (R² ≈ 0.005–0.007) — leveraged non-linear thresholds, robust to missing values.
    - **Neural network (MLP)** (R² ≈ 0.0098) — strongest nonlinear learner, but computationally heavier and less stable out-of-sample.
- **Key takeaway**: demonstrated how different model classes capture different levels of nonlinear signal in noisy financial markets; highlighted importance of **time-based validation, outlier control, and robust preprocessing** for building realistic trading models.

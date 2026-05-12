# Hybrid Quant Forecasting

A research-grade benchmark for financial time-series forecasting using classical econometrics, machine learning, and deep learning hybrid models.

## Research Questions

1. Do hybrid models outperform ARIMA/GARCH/Prophet/XGBoost baselines?
2. How stable are models across market regimes (calm/trending/crash)?
3. Do exogenous features (macro/sentiment) improve robustness?

## Models

### Statistical Baselines
- ARIMA
- GARCH
- Prophet

### Machine Learning
- XGBoost
- Random Forest
- LightGBM

### Deep Learning
- LSTM
- GRU
- Temporal CNN

### Hybrid
- ARIMA + XGBoost (residual modelling)
- GARCH + LSTM

## Datasets

- **Bitcoin OHLCV** — Binance / Coinbase API
- **Equities** — Yahoo Finance
- **Macro** — FRED / VIX

## Evaluation Metrics

- RMSE / MAE / Directional Accuracy
- Regime-wise performance breakdown
- Sharpe ratio / Max drawdown backtests

## Repo Structure

```
hybrid-quant-forecasting/
├── README.md
├── docs/
│   ├── project_overview.md
│   ├── methodology.md
│   ├── data_plan.md
│   ├── modeling_plan.md
│   ├── evaluation_plan.md
│   ├── roadmap.md
│   └── references.md
├── notebooks/
│   ├── 01_eda_template.ipynb
│   ├── 02_feature_engineering_template.ipynb
│   ├── 03_baselines_template.ipynb
│   ├── 04_hybrid_models_template.ipynb
│   └── 05_evaluation_template.ipynb
├── src/
│   ├── data/
│   ├── features/
│   ├── models/
│   ├── evaluation/
│   └── utils/
├── configs/
│   ├── assets.yaml
│   ├── experiments.yaml
│   └── metrics.yaml
└── reports/
    ├── figures/
    └── tables/
```

## Roadmap

| Phase | Focus | Status |
|-------|-------|--------|
| 1 | Data pipeline + baselines (ARIMA/GARCH) | Planned |
| 2 | ML models (XGBoost/RF/LightGBM) | Planned |
| 3 | Deep learning (LSTM/GRU/Transformers) | Planned |
| 4 | Hybrid residual/regime models | Planned |
| 5 | LLM sentiment layer | Planned |
| 6 | Full evaluation + research report | Planned |

## Positioning

This repository serves as a **research-grade benchmark** for comparing classical econometrics against modern ML and hybrid approaches on financial time series. Focus is on real market data only — no synthetic datasets.

## License

MIT

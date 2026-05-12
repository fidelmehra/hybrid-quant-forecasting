# Evaluation Plan

## Metrics

### Point Forecast Metrics
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- MAPE (Mean Absolute Percentage Error)
- Directional Accuracy (%)

### Financial Metrics
- Sharpe Ratio
- Maximum Drawdown
- Annualised return from signal-based backtest

## Regime-Stratified Evaluation

All models evaluated separately on:
- **Calm regime**: Low volatility, sideways market
- **Trending regime**: Sustained directional movement
- **Crash regime**: High volatility, sharp drawdowns

## Statistical Tests
- Diebold-Mariano test for forecast accuracy comparison
- Model Confidence Set (MCS) for ranking models

## Backtesting
- Simple long/short strategy based on directional signal
- Transaction costs included
- Out-of-sample test period: final 20% of data

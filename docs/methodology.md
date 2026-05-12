# Methodology

## Pipeline Overview

1. Data acquisition and cleaning
2. Feature engineering (technical, exogenous, text-derived)
3. Train/validation/test split (walk-forward cross-validation)
4. Model training per asset and regime
5. Hybrid residual/regime model construction
6. Evaluation and comparison

## Walk-Forward Validation

All models use walk-forward validation to avoid look-ahead bias. Training window expands iteratively.

## Hybrid Modelling Strategy

- **ARIMA + XGBoost**: Fit ARIMA, pass residuals to XGBoost for non-linear correction
- **GARCH + LSTM**: Use GARCH for volatility modelling, LSTM for directional signal

## Regime Detection

Market regimes (calm, trending, crash) identified via Hidden Markov Models or rolling volatility thresholds to enable regime-stratified evaluation.

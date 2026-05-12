# Modeling Plan

## Phase 1: Statistical Baselines
- ARIMA (auto-order selection via AIC)
- GARCH(1,1) for volatility
- Prophet for trend/seasonality decomposition

## Phase 2: Machine Learning
- XGBoost with lag features
- Random Forest with feature importance analysis
- LightGBM for efficiency at scale

## Phase 3: Deep Learning
- LSTM (univariate and multivariate)
- GRU (lighter alternative to LSTM)
- Temporal CNN (dilated causal convolutions)

## Phase 4: Hybrid Models
- **ARIMA + XGBoost**: Fit ARIMA on series, model residuals with XGBoost
- **GARCH + LSTM**: Volatility-scaled LSTM inputs from GARCH estimates

## Phase 5: LLM Sentiment Layer
- Integrate news/social sentiment scores as exogenous features
- Fine-tune lightweight LLM embeddings for financial text

## Hyperparameter Tuning
- Grid search / Bayesian optimisation (Optuna)
- Walk-forward validation to prevent data leakage

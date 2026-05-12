# Data Plan

## Sources

| Asset | Source | Frequency |
|-------|--------|-----------|
| Bitcoin OHLCV | Binance / Coinbase API | Daily / Hourly |
| Equities | Yahoo Finance (yfinance) | Daily |
| VIX | Yahoo Finance | Daily |
| Macro indicators | FRED API | Monthly/Daily |

## Features

### Price-Derived
- Returns, log-returns
- Rolling mean, std, min, max
- RSI, MACD, Bollinger Bands
- Order-book depth (where available)

### Exogenous
- Interest rates, inflation-linked variables
- Dollar index
- Equity index spillovers
- Macro announcements
- Crypto on-chain metrics (where relevant)

### Text / AI-Derived
- Sentiment scores
- Topic intensity
- LLM summary embeddings

## Data Quality

- No synthetic data
- Handle missing values via forward-fill or interpolation
- Outlier detection via z-score and IQR methods

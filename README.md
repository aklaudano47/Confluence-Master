# Confluence Signal Engine — Real Gaussian + Real Hull + ATR Trail (Pine Script v6)

A modular TradingView indicator framework that generates **bull/bear confluence scores** from atomic conditions and overlays customizable, non-repainting signals on price charts.

## Core Features
- **Recursive Gaussian Weighted MA (GWMA)** for adaptive smoothing
- **Real Hull Moving Average (HMA)** for momentum regime detection
- **ATR Trail** for trend state initialization
- Configurable **5-of-6 confluence threshold**
- Early-bar safety guards to prevent phantom signals

## Confluence Logic (Per Side)
Each regime evaluates 6 conditions:
1. ATR trail trend state (bull/bear)
2. Candle direction (close > open / close < open)
3. Rising volume vs previous bar
4. Price position vs Gaussian MA
5. Price position vs Hull MA
6. Prior-bar momentum state

A signal prints when the selected threshold (≥5 by default) is met.

## Performance Philosophy
Designed to behave like a **real derivatives research tool**:
- Uses only current and past bar data
- No multi-timeframe lookahead or repainting `security()` calls
- Logic is auditable, extendable, and optimized for live execution

## Usage
1. Open TradingView
2. Launch **Pine Editor**
3. Paste the script
4. Click **Save**
5. Publish as **Idea** or **Public Script** to share your work

## Ideal For
- Crypto and commodity derivatives traders
- Indicator prototyping and rule-based signal research
- Institutional or academic confluence validation

## License
MIT — Free to audit, extend, and experiment with.

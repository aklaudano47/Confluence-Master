# Confluence Signal Engine — Real Gaussian + Real Hull + ATR Trail (Pine Script v6)

A modular, **non-repainting TradingView indicator** that calculates bull/bear confluence scores by combining multiple filtered conditions and overlays signals and custom colored candles directly on the chart.

---

## Core Features

- **Real Gaussian Weighted Moving Average (GWMA)** for adaptive smoothing  
- **Real Hull Moving Average (HMA)** for momentum regime detection  
- **ATR Trail** to define trend direction reliably  
- **Configurable confluence score threshold** (up to 6)  
- **Custom candles & background tinting options**  
- Signal markers and alert conditions built-in  
- Logic designed for reproducible research and live use  

---

## Confluence Logic (Per Side)

Each bar is evaluated across 6 conditions:

1. ATR trend state (bull / bear)  
2. Price candle direction  
3. Rising volume  
4. Price above/below Gaussian MA  
5. Price above/below Hull MA  
6. Trend direction of Hull MA

A *bull* or *bear* signal is shown when the confluence count meets or exceeds the specified threshold.

---

## Designed for Real Market Use

- Uses only current & historical bar data  
- Avoids lookahead bias and repainting functions (`security()`)  
- Fully auditable, extendable, and optimized for TradingView v6  
- Includes alerts, overlays, and UX toggles for flexible usage

---

## How to Use

1. Open **TradingView**  
2. Open the **Pine Editor** panel  
3. Paste the script  
4. Save & **Add to Chart**  
5. Optionally publish to your TradingView ideas or scripts

If you want others to view the script on TradingView, you can publish it as an *Idea*, *Protected Script*, *Invite-Only*, or *Public Script* there. :contentReference[oaicite:0]{index=0}

---

## Ideal For

- Crypto / commodities derivatives traders  
- Researchers needing modular confluence signals  
- Indicator prototyping and validation  
- Quantitative analysis workflows

---

## License

MIT License — free to audit, extend, and experiment with.

---

# ARPS Ultra Scalper Trading Script

The **ARPS Ultra Scalper** is an advanced TradingView script that integrates multiple indicators and chart patterns to provide reliable trading signals for scalpers and short-term traders. This script is designed to assist traders in identifying high-probability trade setups based on a combination of trend indicators, candle patterns, and custom logic.

## Features

### 1. **RSI-Based Signals**
- Uses the RSI (Relative Strength Index) combined with Weighted Moving Averages (WMA) to detect trend direction and momentum shifts.
- Crossover signals based on RSI and WMA interactions.

### 2. **Stochastic Oscillator**
- Incorporates a smoothed Stochastic Oscillator (`%K` and `%D`) to refine entry and exit points.
- Provides additional checks during overbought/oversold conditions.

### 3. **Candle Pattern Recognition**
The script identifies key candlestick patterns, including:
- **Doji Variants**: Regular, Flying Dragon, and Gravestone Doji.
- **Morning Star** and **Evening Star** Reversal Patterns.
- **Hammer** and **Shooting Star**.
- **Engulfing Patterns**: Bullish and Bearish Engulfing.
- **Harami Patterns**: Bullish and Bearish Harami.
- **Dark Cloud Cover**: A strong bearish reversal indicator.

### 4. **Ichimoku Cloud Integration**
- Configurable Ichimoku Cloud with adjustable parameters for Tenkan-Sen, Kijun-Sen, Senkou Span A/B, and displacement for Chikou Span.
- Enhanced feature of dual-cloud logic with finer granularity (e.g., Ichimoku with "adjust and double").
- Cloud-based buy/sell signals using crossovers and above/below the cloud logic.

### 5. **Parabolic SAR**
- Incorporates the Parabolic SAR (Stop and Reverse) to determine market direction.
- Provides confirmation for trend continuation or reversals.

### 6. **Trend Continuation Factor (TCF)**
- Innovative calculation of the Plus and Minus TCF to gauge the strength of the ongoing trend.
- Enhances the robustness of signal generation.

### 7. **Entry and Exit Signals**
- **Buy Signals**:
	- Bullish RSI-Stochastic crossovers.
	- Bullish crossovers of moving averages (WMA).
	- Bullish candlestick pattern detected.
	- Above Ichimoku Cloud with trend confirmation.
- **Sell Signals**:
	- Bearish RSI-Stochastic crossovers.
	- Bearish crossovers of moving averages (WMA).
	- Bearish candlestick pattern detected.
	- Below Ichimoku Cloud with trend confirmation.
- Visual aids with `Long Position` and `Short Position` labels.

### 8. **Alerts**
- Alerts are configured to notify you of Buy or Sell signals in real-time, so you never miss an opportunity.

---

## How the Script Works

1. **Indicator Logic**:
   - The script intelligently combines multiple indicators (e.g., RSI, WMA, Stochastics, Parabolic SAR) to assess both trend direction and momentum.
   - Custom logic integrates bullish and bearish candlestick patterns with Ichimoku analysis for thorough signal evaluation.

2. **Candle Pattern Detection**:
   - The script evaluates historical patterns (`[1]` or `[2]` candles back) and current candles to identify reversal areas.

3. **Filtering False Signals**:
   - False positives are reduced through cloud confirmation and Parabolic SAR checks.

4. **Signal Confirmation**:
   - Trade signals (Buy/Sell) occur only when multiple conditions align, improving signal reliability.

---

## Parameters (Configurable Inputs)

- **Length**: Used for trend durations across indicators (default: 20).
- **Source**: Price source (default: `close`).
- **RSI Length**: Adjustable periods for RSI calculation.
- **Stochastic K, D, and Smoothing**: Fine-tune oscillator behavior.
- **Ichimoku Parameters**: Customize periods for Tenkan-Sen, Kijun-Sen, and Senkou Span B.
- **Candlestick Pattern Sensitivity**:
	- Doji Size (default: 0.03).
  
---

## Visualization

- **Buy Positions**: Highlighted with green labels and upward-pointing arrows.
- **Sell Positions**: Highlighted with red labels and downward-pointing arrows.
- **Ichimoku Cloud**:
  - **Green Cloud** when bullish (Senkou Span A > Senkou Span B).
  - **Red Cloud** when bearish (Senkou Span A < Senkou Span B).

---

## Use Cases

- **Scalping**: Quickly detect short-term reversal setups.
- **Intraday Traders**: Utilize Ichimoku confirmations and pattern recognition for day trading.
- **Trend-Continuation Strategies**: Leverage TCF and Parabolic SAR for momentum trading.

---

## How to Use

1. Copy and paste the code into the Pine Script editor on TradingView.
2. Customize the input settings based on your trading preferences.
3. Apply the script to any chart (e.g., cryptocurrency, forex, stocks).
4. Monitor generated signals or set up alerts to receive notifications.

---

## Alerts

- Configurable alerts for Buy and Sell signals ensure you receive real-time notifications.
  - Example message: `"Buy Signal identified. Entry opportunity detected!"`

---

## Disclaimer

The ARPS Ultra Scalper is a powerful trading assistant but does **not guarantee profits**. Always backtest and validate based on your trading style and risk tolerance. Use it as a supportive tool alongside other trading strategies.

---

Feel free to reach out for further enhancements or questions about the script. Happy trading!
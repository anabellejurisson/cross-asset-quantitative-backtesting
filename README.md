# SPY Quantitative Backtesting Strategy

## Executive Summary
This repository contains a systematic trend-following research backtest implemented in **Pine Script (v5)** for the SPDR S&P 500 ETF Trust (**$SPY**). 

---

## Strategy Backtest Results (1993 – 2026)

| Performance Metric | Backtest Value |
| :--- | :--- |
| **Initial Capital** | $10,000.00 |
| **Total Net Profit** | +$84,663.93 (+846.64%)[cite: 7] |
| **Max Drawdown** | 20.15% ($8,661.15)[cite: 7] |
| **Profit Factor** | 2.921[cite: 7] |
| **Win Rate** | 33.64% (37/110 trades)[cite: 7] |

---

## Strategy Rules & Mechanics
* **Trend Filter:** 200-day Simple Moving Average (SMA).
* **Entry Signal:** Price crosses above the 200-day SMA (`ta.crossover`)[cite: 6].
* **Exit Signal:** Price crosses below the 200-day SMA (`ta.crossunder`)[cite: 6].
* **Execution Parameters:** 100% equity position sizing per signal.

---

## Repository Structure
* `trend-following-strategy.pine` — Main TradingView Pine Script (v5) backtesting engine[cite: 5].
* `README.md` — Performance overview and implementation notes[cite: 3, 5].

---

## How to Reproduce in TradingView
1. Copy the code from `trend-following-strategy.pine`[cite: 5].
2. Open TradingView, navigate to the **Pine Editor** tab at the bottom, and paste the code.
3. Click **Add to chart** and apply to daily timeframe for **$SPY**.

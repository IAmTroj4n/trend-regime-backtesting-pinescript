# trend-regime-backtesting-pinescript

This repository contains a learning-focused, rule-based trading strategy implemented in Pine Script v6:

-The project demonstrates how a discretionary technical idea (EMA-based trend regimes with Supply/Demand zones) can be converted into a deterministic, backtestable trading system.
-The primary goal is methodology: preserving intent, removing ambiguity, and enabling objective evaluation through backtesting.
-This serves as a baseline system for further experimentation, statistical analysis, and future extensions such as risk management and modeling layers.

# EMA Regime + Supply/Demand Backtest (Pine Script v6)

This repository contains a **learning-oriented quantitative trading project** that converts a visual trading indicator into a **fully backtestable strategy** using Pine Script v6.

The focus of this project is methodological correctness', not signal optimization or profitability.

---

## Objectives:

In quantitative trading, trading ideas must be:
1. Explicitly defined
2. Deterministic
3. Objectively testable

This project demonstrates how to:
- Take a discretionary technical concept
- Preserve its original logic
- Convert it into a systematic, backtestable trading strategy

---

##  Strategy Overview

### Core Components
- **EMA (10/21) Trend Regime**
  - Identifies bullish and bearish market regimes
  - Trend state is persistent, not crossover-based
- **Trend-Shift Entries**
  - Trades are triggered only when the regime changes
- **Supply & Demand Zones**
  - Detected using pivot-based swing logic
  - Visual only (not used for trade filtering or exits)

### Trade Characteristics
- Always-in-market regime-switching system
- No stop loss or take profit
- Positions flip only on regime change
- Designed to evaluate trend persistence behavior


## Implementation Details

- Language: **Pine Script v6**
- Script Type: `strategy()`
- Logic: Identical to original indicator
- Backtesting: TradingView Strategy Tester
- No additional filters, indicators, or risk rules added

All `if` conditions are explicitly boolean-compliant (v6-safe).

---

## What The Project is about:

### This is:
- A clean baseline strategy
- A learning-focused quant project
- A demonstration of systematic thinking
- Suitable for academic, internship, and portfolio use

## NOT A PRODUCTION GRADE INDICATOR USED FOR TRADING

---


---

## Disclaimer

This repository is for **educational and research purposes only**.  
No financial or investment advice is provided.

---

## Contributions & Discussion

Feedback, discussions, and methodological critiques are welcome especially around:
- Regime definitions
- Backtesting assumptions
- Strategy evaluation metrics

# Evaluating LLM Strategy Generation via R Backtesting

An empirical evaluation comparing LLM-generated tactical trading strategies against Modern Portfolio Theory (MPT) dynamic asset allocation using a standardized R backtesting framework.

## Key Findings

* **MPT Dynamic Allocation (Top Performer):** Achieved an annualized **Sharpe Ratio of 0.81** and limited Maximum Drawdown to **9.40%** under weekly 5% threshold rebalancing.
* **LLM Tactical Baseline (`AI_Aggressive`):** Outperformed other AI variants with a **Sharpe Ratio of 0.34** and Max Drawdown of **14.49%**.
* **Friction & Drift:** Transaction costs (10 bps) and price drift significantly eroded unconstrained AI strategy returns, proving the necessity of portfolio optimization constraints.

## Repository Structure

* `Evaluating LLM Strategy Generation.Rmd`: Executable R code covering ETF data ingestion (SPY/AGG/BIL), quadprog optimization, tactical signal logic, and backtesting.
* `Project Report.pdf`: Full research paper detailing baseline methodology, 2022 regime stress testing, and sensitivity analysis.

## Core Stack & Tools

* **Language:** R
* **Key Packages:** `xts`, `quantmod`, `quadprog`, `PerformanceAnalytics`

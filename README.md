# Managing Linear Risk in International Trade

## Project Overview
This project focuses on analyzing and managing linear risk in foreign exchange, specifically for the GBP/USD currency pair. The analysis includes calibrating exchange rate processes, calculating Value at Risk (VaR) for unhedged and hedged positions, and exploring alternative hedging strategies using ETFs.

## Objectives
1. Calibrate the exchange rate process for GBP/USD
2. Calculate VaR for unhedged positions
3. Analyze the effectiveness of unitary hedging strategies
4. Explore ETF-based hedging alternatives

## Tools and Techniques
- R programming language
- Monte Carlo simulation
- Yahoo Finance API for historical data
- Risk metrics calculation (VaR)
- Time series analysis
- ETF screening and analysis

## Key Components

### 1. Calibrating the Exchange Rate Process
- Estimated theta using forward quotes and interest rate parity
- Compared calibrated theta with LIBOR rates
- Calibrated sigma (volatility) using historical GBP/USD exchange rate data

### 2. VaR for Unhedged Positions
- Implemented Monte Carlo simulation to model future exchange rates
- Calculated 99% VaR for unhedged exporter position

### 3. Unitary Hedge Analysis
- Simulated futures contract prices using interest rate parity
- Calculated 99% VaR for hedged positions using:
  a) Futures contract expiring in December 2024
  b) Futures contract expiring in September 2024
- Analyzed the impact of basis risk on hedging effectiveness

### 4. ETF-based Hedging Strategies
- Screened 5 different ETFs as potential hedging instruments
- Provided economic rationale for each ETF's suitability as a GBP/USD hedge
- Reported hedge effectiveness using beta values

## Key Findings

1. Calibrated Exchange Rate Parameters:
   - Theta (interest rate differential): 0.05359
   - Sigma (volatility): 0.08552515

2. VaR Results:
   - Unhedged 99% VaR: $214,840
   - Hedged 99% VaR (Dec 2024 futures): $7,426.08
   - Hedged 99% VaR (Sep 2024 futures): $23,109.10

3. Hedging Effectiveness:
   - Unitary hedging significantly reduces risk compared to unhedged positions
   - Matching futures contract maturity to cash flow timing minimizes basis risk

4. ETF Hedging Alternatives:
   - Direct currency ETFs (e.g., FXB) provide the most effective hedge
   - Equity-based ETFs (e.g., EWU, HEDJ) offer moderate hedging effectiveness
   - Commodity ETFs (e.g., GLD) provide minimal hedging effectiveness

## Conclusions
- Proper calibration of exchange rate processes is crucial for accurate risk assessment
- Hedging strategies can significantly reduce VaR, with futures contracts matching cash flow timing being most effective
- ETFs can serve as alternative hedging instruments, but their effectiveness varies based on the underlying assets and economic relationships

## Future Work
- Explore dynamic hedging strategies that adjust based on market conditions
- Incorporate transaction costs and margin requirements into hedging analysis
- Investigate the impact of macroeconomic factors on hedging effectiveness
- Analyze the performance of hedging strategies under different market regimes (e.g., high volatility, trending markets)

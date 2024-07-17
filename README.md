

# Mean-Reversion - VIX Breakout Trading Strategy

## Overview
This repository contains a Python implementation of a trading strategy that capitalizes on volatility signals from the VIX (CBOE Volatility Index) to trade SPY (S&P 500 ETF). The strategy aims to enter long positions when the VIX breaks above its upper Bollinger Band and exit based on a momentum indicator in SPY.

### Strategy Components:
- **Signal Generation:** 
  - Calculate Bollinger Bands for the VIX using a 20-day moving average and standard deviation.
  - Generate buy signals when the VIX closes above its upper Bollinger Band.
  - Shift these signals to the next day to align with SPY's opening price.

- **Exit Strategy:** 
  - Exit positions in SPY after observing two consecutive days of upward momentum in closing prices.

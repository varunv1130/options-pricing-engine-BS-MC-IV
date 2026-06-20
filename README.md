# options-pricing-engine-BS-MC-IV
# Options Pricing Engine

A Python implementation of options pricing methodologies, 
calibrated to live market data.

## What this does

- **Black-Scholes pricer** with full Greeks (delta, gamma, vega, theta)
- **Monte Carlo simulation** engine for path-dependent exotic options 
  (Asian calls, barrier options) using vectorised GBM
- **Implied volatility surface** calibrated to live SPY options data, 
  with vol smile and skew analysis

## Key findings (June 2026)

SPY ATM implied vol is ~15%, roughly in line with 30-day realised vol 
of 15.24%, suggesting options are fairly priced with no strong 
structural edge for buyers or sellers. The put skew is moderate, 
consistent with the VIX having normalised from a spike of 31 in 
March 2026.

See `writeup.txt' for full market analysis.

## Tech stack

Python — NumPy, SciPy, Matplotlib, yfinance  
Environment: Google Colab

## Files

- `Options Pricing Engine.ipynb` — full notebook with all three stages
- `writeup.txt` — one-page market analysis writeup

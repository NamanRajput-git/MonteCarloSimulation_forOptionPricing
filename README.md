# Monte Carlo Option Pricing Using Real Market Data

## Project Overview

This project implements a Monte Carlo simulation framework to price European options based on historical market data. It compares Monte Carlo prices with Black-Scholes analytical prices and actual market mid-prices. Variance reduction techniques, such as antithetic variates and control variates, are applied to improve the accuracy and convergence of the Monte Carlo simulation.

The project also provides tools for analyzing errors, visualizing pricing discrepancies across strikes, and performing sensitivity analysis by moneyness and volatility.

## Features

- Download historical underlying stock prices (via Yahoo Finance API).
- Extract option chain data for selected expiries.
- Estimate historical and implied volatilities.
- Monte Carlo simulation for European call options:
  - Risk-neutral Geometric Brownian Motion model
  - Antithetic variates
  - Control variates using Black-Scholes analytical price
- Comparison with market mid-prices and Black-Scholes prices.
- Calculation of standard errors and 95% confidence intervals.
- Analysis and visualization of errors across strikes and moneyness.
- 
## Key Parameters
 - S0: Spot price of underlying at evaluation date.
 - K: Strike prices of options.
 - T: Time to expiry in years.
 - r: Risk-free interest rate (annual).
 - q: Dividend yield (annual).
 - sigma: Volatility (historical or implied).
 - n_paths: Number of Monte Carlo simulation paths.
 - n_steps: Number of time steps for path discretization.

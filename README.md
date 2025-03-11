PFE Analysis for Power Purchase Agreements (PPA)
Project Overview

This repository contains a Monte Carlo simulation framework for estimating the Potential Future Exposure (PFE) of a Power Purchase Agreement (PPA). The goal is to assess the financial risks associated with electricity price fluctuations over time and compare the estimated exposure to real historical market developments.
Methodology

    Data Collection:
        Import historical electricity market prices from SMARD.de.
        Clean and preprocess the dataset for model calibration.

    Price Modeling:
        Apply an Ornstein-Uhlenbeck process with jumps to simulate electricity price evolution.
        Estimate model parameters (mean reversion, volatility, jump intensity) based on historical data.

    Monte Carlo Simulations:
        Generate multiple future price trajectories to capture uncertainty.
        Compute the Potential Future Exposure (PFE) over different time horizons.

    Risk Analysis:
        Compare the simulated exposure to historical price developments.
        Assess potential financial risks in a fixed-price PPA scenario.

Data Source

    Market Data: SMARD.de - German Electricity Market Data
    Historical electricity prices are used to calibrate the Ornstein-Uhlenbeck model and validate the Monte Carlo simulation.

Results & Insights

    The simulated electricity prices exhibit a range of possible future outcomes, incorporating extreme price shocks and market fluctuations.
    The PFE grows over time, highlighting potential financial exposure risks in a long-term PPA.
    Results suggest that hedging strategies and contract flexibility could mitigate financial risks.

Possible Next steps

🔹 Enhance the model with seasonal components to better reflect cyclical electricity price trends.
🔹 Compare Monte Carlo forecasts with alternative models (e.g., GARCH, LSTM, or reinforcement learning-based predictions).

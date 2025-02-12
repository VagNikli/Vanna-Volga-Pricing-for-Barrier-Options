# Vanna-Volga-Pricing-for-Barrier-Options

## Overview
This project implements the **Vanna-Volga method** for pricing exotic **Foreign Exchange (FX) barrier options**, expanding on the **Black-Scholes model** by incorporating volatility adjustments to better align with market conditions. The implementation supports both **vanilla options** and **barrier options**, including **up-in, up-out, down-in, and down-out** structures.

## Objective
The goal of this project is to:
- Compute **vanilla** and **barrier** option prices using the **Black-Scholes** and **Vanna-Volga** methods.
- Model the impact of **volatility risk** on option pricing.
- Provide a flexible **Python-based implementation** for different option structures.
- **Visualize** the effect of barriers on option prices.

## Project Structure

Vanna-Volga-Barrier-Options/
│── src/
│   ├── fx_barrier_option.py  # Core implementation
│   ├── vanna_volga.py        # Vanna-Volga adjustments
│   ├── visualization.py      # Plotting functions
│── notebooks/
│   ├── pricing_demo.ipynb    # Jupyter notebook with usage examples
│── tests/
│   ├── test_fx_barrier_option.py  # Unit tests
│── requirements.txt   # Dependencies
│── README.md          # Project documentation
│── LICENSE            # License (MIT, etc.)
│── .gitignore         # Ignore unnecessary files




## Methodology
The **Vanna-Volga approach** enhances the **Black-Scholes model** by adjusting option pricing based on market-implied volatilities. The implementation consists of the following steps:

1. **Define Option Parameters**:
   - **Spot price (S)**
   - **Strike price (K)**
   - **Time to maturity (T)**
   - **Volatility (σ)**
   - **Domestic & foreign risk-free rates**
   - **Barrier level (if applicable)**

2. **Compute Vanilla Option Price**:
   - Use the **Black-Scholes formula** for European **call and put** options.
   - Calculate **d1** and **d2** terms.

3. **Compute Barrier Option Price**:
   - Implement barrier conditions using mathematical adjustments.
   - Support **up-in, up-out, down-in, down-out** options.

4. **Apply Vanna-Volga Adjustments**:
   - Derive risk-neutral pricing corrections for market consistency.
   - Compute adjusted prices for exotic options.

5. **Visualization**:
   - Compare vanilla and barrier option prices as **spot price varies**.
   - Demonstrate the impact of **barriers** on option value.

## Installation & Usage
### Requirements
Ensure you have Python installed with the required libraries:

```bash
pip install -r requirements.txt


# Factor-Based Portfolio Optimization and Strategy Backtesting

This project develops a **systematic portfolio optimization framework** to evaluate how different covariance and expected return estimators affect portfolio performance across market regimes. The framework applies **factor-based return estimation and mean–variance optimization** to construct and evaluate long-only and long-short ETF portfolios.

The analysis studies estimator sensitivity and portfolio performance across **pre-crisis, crisis, and post-crisis market environments**.

---

## Project Objectives

- Construct optimized portfolios using **mean–variance optimization**
- Estimate expected returns using **factor-based models**
- Analyze **estimator sensitivity across market regimes**
- Compare **long-only and long-short portfolio strategies**
- Evaluate performance using **risk-adjusted metrics**

---

## Methodology

### Portfolio Optimization

Portfolio weights are estimated using a **mean–variance optimization framework**:

max(wᵀμ − λ wᵀΣw)

Where:

- μ = expected returns  
- Σ = covariance matrix  
- λ = risk-aversion parameter  

Optimization is implemented using **Python and CVXPY**.

---

### Factor-Based Return Estimation

Expected returns are estimated using the **Fama–French Three-Factor Model**:

Ri − Rf = α + βm(Mkt−Rf) + βsSMB + βvHML + ε

This model captures exposure to:

- Market risk
- Size factor (SMB)
- Value factor (HML)

---

## Strategy Construction

Two portfolio strategies are evaluated.

### Long-Only Strategy
- Portfolio weights constrained to positive values
- Diversified exposure across ETFs

### Long-Short Strategy
- Allows short selling
- Enables hedging during volatile market conditions

---

## Backtesting Framework

Portfolio strategies are evaluated using a **rolling backtesting framework with periodic rebalancing**.

Performance is analyzed across multiple market regimes:

- Pre-Crisis Period
- Financial Crisis Period
- Post-Crisis Recovery

---

## Risk and Performance Metrics

Portfolio performance is evaluated using:

- Sharpe Ratio
- Volatility
- Maximum Drawdown
- Skewness
- Kurtosis
- Value at Risk (VaR)
- Conditional Value at Risk (CVaR)

---

## Key Findings

- Long-short strategies produced **significantly higher risk-adjusted returns** compared to long-only portfolios.
- Portfolio performance is **highly sensitive to the choice of covariance and expected return estimators**.
- Short-term estimators adapt quickly to market changes but introduce **higher estimation noise**.
- Long-term estimators provide **more stable portfolio allocations during recovery periods**.

These results highlight the importance of **estimator selection in systematic portfolio construction**.

---

## Repository Structure

```
factor-based-portfolio-optimization/
│
├── notebook/
│   └── code_factor_portfolio.pdf
│
├── report/
│   └── report_factor_portfolio.pdf
│
└── README.md
```

### notebook/
Contains the implementation notebook describing:

- data preprocessing  
- factor model estimation  
- portfolio optimization  
- backtesting framework  
- strategy evaluation  

### report/
Contains the full research report detailing:

- methodology  
- empirical analysis  
- results  
- conclusions

---

## Technologies Used

- Python
- Pandas
- NumPy
- CVXPY
- Matplotlib

---

## Applications

This project demonstrates techniques used in:

- Quantitative portfolio construction
- Systematic investing strategies
- Factor-based asset allocation
- Portfolio risk analytics

---

## Author

**Mrinal Gupta**  
MS Financial Engineering  
Stevens Institute of Technology

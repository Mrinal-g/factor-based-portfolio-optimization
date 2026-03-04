# Factor-Based Portfolio Optimization and Strategy Backtesting

This project implements a factor-based portfolio optimization and strategy evaluation framework using mean–variance optimization and the Fama–French three-factor model. The system constructs and evaluates long-only and long-short ETF portfolios through a rolling backtesting framework and analyzes strategy performance using risk-adjusted metrics.

---

## Project Type

Applied quantitative finance project focused on **portfolio analytics, optimization, and strategy backtesting** using factor models.

---

## Project Objectives

- Construct optimized portfolios using **mean–variance optimization**
- Estimate expected returns using **factor-based models**
- Implement **long-only and long-short portfolio strategies**
- Evaluate portfolio performance through **rolling backtesting**
- Compare strategies using **risk-adjusted performance metrics**

---

## Methodology

### Portfolio Optimization

Portfolio weights are estimated using a **mean–variance optimization framework**:

max ( wᵀ μ − λ wᵀ Σ w )

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

Performance is evaluated using a **rolling backtesting framework with periodic rebalancing** to assess portfolio behavior across different market conditions.

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

- Long–short portfolios achieved higher **risk-adjusted returns** compared to long-only strategies.
- Portfolio performance depends strongly on the **risk and return estimates used in the optimization process**.
- Allowing short positions improves diversification and enables better hedging during volatile market conditions.

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

## Libraries Used

- Python
- Pandas
- NumPy
- CVXPY
- Matplotlib

---

## Applications

This project demonstrates techniques commonly used in:

- Quantitative portfolio construction
- Systematic asset allocation
- Portfolio analytics and performance evaluation
- Factor-based investment strategies

---

## Author

**Mrinal Gupta**  
MS Financial Engineering  
Stevens Institute of Technology

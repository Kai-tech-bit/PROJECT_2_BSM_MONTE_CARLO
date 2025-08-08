# 📉 Black-Scholes Option Pricing & Monte Carlo Simulation for Risk Analysis

## 📌 Overview
This project implements **closed-form and simulation-based option pricing models** to evaluate and compare theoretical valuations with stochastic simulation outputs. The work blends **analytical finance** with **numerical methods** to assess pricing accuracy, explore model limitations, and demonstrate extensions toward more realistic market dynamics.

---

## 🎯 Objectives
- Implement the **Black-Scholes-Merton (BSM)** closed-form pricing formula for European call and put options.
- Compute **Greeks** (Δ, Γ, Θ, 𝜈, ρ) using:
  - **Closed-form analytical expressions**
  - **Monte Carlo simulation with finite-difference estimation**
- Perform **Monte Carlo path simulations** for underlying asset price dynamics.
- Compare pricing accuracy between analytical and simulation-based methods.
- Explore **model shortcomings** and visualise:
  - Volatility smile
  - Volatility skew
  - Simulated paths from **Heston** and **Jump-Diffusion** models.

---

## 🛠️ Tech Stack
- **Python** — Model implementation & simulations
- **Libraries**: `numpy`, `scipy`, `matplotlib`, `seaborn`, `pandas`
- **Mathematical Models**: Black-Scholes-Merton, Geometric Brownian Motion, Heston, Jump-Diffusion

---

## 📊 Key Analysis Steps
1. **Closed-Form Pricing**  
   - Black-Scholes formula for European calls & puts.
   - Inputs: Spot price (S), Strike (K), Time to maturity (T), Volatility (σ), Risk-free rate (r).

2. **Monte Carlo Pricing**  
   - Simulate thousands of underlying price paths.
   - Apply risk-neutral valuation to estimate option prices.
   - Use **Law of Large Numbers** to improve convergence.

3. **Greeks Calculation**  
   - **Closed-form**: Direct differentiation of BSM formulas.
   - **Simulation**: Finite difference approach using perturbed payoffs.

4. **Comparative Analysis**  
   - Analytical vs Simulation price differences.
   - Impact of number of simulations & volatility changes.

5. **Model Shortcomings**  
   - Volatility smile & skew phenomena.
   - Market frictions not captured by BSM assumptions.
   - Extensions using stochastic volatility (Heston) & jumps.

---

## 📈 Results Summary
- **Monte Carlo estimates** converge to closed-form prices with sufficiently large path counts.
- **Finite-difference Greeks** closely match analytical results but show higher variance for small simulation sizes.
- **Volatility smile and skew** highlight BSM’s inability to capture implied volatility structures observed in real markets.
- **Heston and Jump-Diffusion models** produce more realistic price dynamics.

---



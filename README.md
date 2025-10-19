# MSc Thesis – Separating Strategic Choice from Forecast Error  
**Analytical and Simulation Insights into Dutch Imbalance Pricing**  
---

## Overview  
This repository contains all materials related to my master’s thesis, **"Separating Strategic Choice from Forecast Error: Analytical and Simulation Insights into Dutch Imbalance Pricing"**, completed within the MSc in Economics program at Tilburg University.

The research investigates how different **imbalance pricing mechanisms** in the Dutch electricity market influence balancing costs and market behaviour. By explicitly disentangling **intentional (strategic)** and **unintentional (stochastic)** deviations, the thesis develops a closed-form feedback model validated by a Monte Carlo simulation.

---

## Abstract  
The growing share of **variable renewable energy (VRE)** has intensified forecast errors, **Area Control Error (ACE)**, and imbalance price volatility across European power systems.  
This work builds a simplified analytical model describing the feedback interaction between **Transmission System Operator (TSO)** reserve activation and **Balancing Responsible Parties (BRPs)** deviations. The model—parameterized with Dutch data—explicitly separates **strategic behavior** from **forecast error**, providing quantitative insights into pricing rules such as:
- Immediate  
- Average  
- End  
- Dual  
- Conditional Dual  

Main findings:  
1. Once a stable feedback equilibrium exists, all predictable components of ACE are eliminated; residual ACE mirrors forecast error shocks.  
2. Pricing design redistributes costs—End pricing shifts cost to TSOs, while Dual/Conditional Dual shifts cost to BRPs.  
3. Policy should prioritize **forecasting improvements** and **battery storage incentives**, as no pricing rule intrinsically reduces ACE variance.

---

## Methods and Implementation  
- **Analytical Framework:** Closed-form feedback model of BRP–TSO interaction under stochastic imbalance.  
- **Simulation:** Monte-Carlo approach in Python (`NumPy`, `SciPy`, `Pandas`, `Matplotlib`) to validate analytical results and perform sensitivity analysis.  
- **Calibration Data:** Dutch imbalance data (TenneT, Sept 2023–2024).  
- **Parameters estimated:** Balancing costs (γ), adjustment costs (θ), persistence (ρ), and variance of shocks (σϵ).

For reproducibility, model classes and calibration routines are documented within the `/code/` directory.

---

## Repository Structure  

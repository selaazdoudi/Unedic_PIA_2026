# Unedic_PIA_2026

## 📌 Project Overview

This project develops a **macro-economic evaluation framework** for the 2023 French unemployment insurance reform, commissioned in collaboration with Unédic (Direction des Études et Analyses).

Unlike standard micro-evaluations, this work focuses on **general equilibrium effects**, using **search-and-matching models** to assess how changes in unemployment insurance (UI) parameters affect labor market outcomes.

The core objective is to analyze whether the reform — which introduces **state-dependent benefit duration** — can effectively:
- Increase employment
- Strengthen job-search incentives
- Reduce recruitment difficulties

The goal of this work is to show qualitatively how unemployment insurance mechanisms transmit into the economy. 

---

## Economic Framework

The project builds on **search-and-matching theory** to model labor market dynamics, including:

- Matching function between workers and firms
- Labor market tightness (θ = vacancies / unemployment)
- Endogenous job search effort
- Wage determination via Nash bargaining
- Vacancy creation by firms

The reform is modeled as a **reduction in expected benefit duration (−25%)**, conditional on labor market conditions.

Two key transmission channels are analyzed:

1. **Incentive channel**  
   Shorter benefit duration increases job search effort before exhaustion.

2. **Bargaining channel**  
   Reduced outside options lower wages, affecting firms’ vacancy posting decisions.

---

##  Model Structure

The repository implements several versions of the model:

### 🔹 Model 1 — Baseline
- Steady-state search-and-matching model
- Endogenous search effort
- Time-limited unemployment benefits

### 🔹 Model 1.5 — Wage Rigidities
- Introduces a binding minimum wage
- Limits wage adjustment through bargaining
- Highlights the role of institutional constraints

### 🔹 Model 2 — Business Cycle Extension
- Multi-state macroeconomic environment
- Endogenous job destruction
- Allows evaluation across economic regimes

---

##  Calibration & Simulation

The model is calibrated to **French labor market data (H2 2022)**.

Simulations compare:
- Pre-reform equilibrium
- Post-reform equilibrium (25% reduction in benefit duration)

Key outcomes analyzed:
- Unemployment rate
- Vacancy creation
- Wage levels
- Matching efficiency

---

## Key Findings

- The reform is **theoretically consistent** with improving employment in tight labor markets  
- However, **quantitative effects remain modest**  
- Stronger search incentives do reduce unemployment, but:
  - Vacancy creation responds weakly
  - Recruitment difficulties are only marginally affected  
- Wage rigidities significantly **dampen firm-side responses**
- The reform induces a **trade-off between employment gains and income protection**

---

##  Repository Structure

Unedic_PIA_2026/
├── notebooks/
│   ├── model_1_benchmark.ipynb
│   ├── model_1.5_wage_rigidities.ipynb
│   └── model_2_business_cycle.ipynb
├── paper/
│   └── research_paper.pdf
└── presentation/

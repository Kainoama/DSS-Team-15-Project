# ML-Based Loan Risk & Pricing Optimization System

A machine learning–driven decision support system that predicts borrower default risk and determines the **profit-maximizing interest rate** using SBA 7(a) loan data.

> **Core Question:**  
> What is the optimal risk-adjusted interest rate that maximizes bank profitability?

---

##  ⚠️  The Problem

Banks face a fundamental trade-off:

- Higher interest rates increase revenue  
- Higher rates also increase default risk and customer churn  

Traditional credit models predict default —  
but they **do not optimize pricing**.

---

## Our Approach

We integrate **Risk Prediction + Financial Modeling + Pricing Simulation** into one unified system.

---

### 1. Predict Default Risk

- Train ML models (XGBoost / Random Forest)  
- Estimate **Probability of Default (PD)**  
- Segment borrowers into Risk Tiers (Low / Medium / High)  
- Identify key risk drivers:
  - Industry (NAICS)
  - Business Age
  - Collateral Status

---

### 2. Integrate Financial Logic

We incorporate the SBA Government Guarantee into Expected Loss:

Expected Loss = PD × LGD × EAD  

Net LGD = LGD × (1 − Guarantee%)

---

### 3. Optimize Interest Rates

We simulate interest rate scenarios and compute:

Expected Profit = Interest Revenue − Expected Loss  

This identifies the **profit-maximizing “sweet spot” rate** by industry segment.

---

## Interactive Strategy Dashboard (Tableau)

Designed for Credit & Strategy Teams:

- Risk Tier Classification  
- Industry Risk Heatmap  
- Feature Importance Analysis  
- Dynamic Profit Curves  
- What-If Interest Rate Simulator  

Users can test rate changes and instantly see portfolio-level profit impact.

---

## Value Proposition

Our system transforms credit risk modeling into a **strategic pricing engine**:

- Quantifies the margin vs. default trade-off  
- Optimizes pricing by industry  
- Leverages SBA guarantees for smarter risk-taking  
- Enables data-driven profitability decisions  

---

## ⏱ 6-Week Execution Plan

| Week(s)   | Focus Area                                   | Key Output |
|------------|----------------------------------------------|------------|
| Weeks 1–2  | Data Engineering & NAICS Grouping            | Cleaned dataset with aggregated industry sectors |
| Week 3     | PD Model Development                         | Trained ML model predicting Probability of Default |
| Week 4     | Financial Integration (SBA Guarantee)        | Risk-adjusted Expected Loss & profit formula |
| Week 5     | Dashboard Development                        | Interactive pricing & risk simulator (Tableau) |
| Week 6     | Strategy Validation & Final Presentation     | Profit comparison vs. historical pricing |

---

## Resources
- **Data source:** U.S. Small Business Administration –  
7(a) & 504 FOIA dataset: FOIA – 7(a) (FY2020-Present) as of 251231 (public domain),  
https://data.sba.gov/en/dataset/7-a-504-foia/resource/d67d3ccb-2002-4134-a288-481b51cd3479 (accessed Month Day, Year). :contentReference[oaicite:1]{index=1}

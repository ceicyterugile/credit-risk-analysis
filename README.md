# Mortgage Credit Risk & Basel III RWA Analysis

## 📌 Project Overview & Business Goal
This project focuses on calculating Credit Risk Risk-Weighted Assets (RWA) and baseline capital requirements for a bank's mortgage portfolio under the **Basel III Regulatory Framework**. 

The strategic goal is to build an analytical data pipeline that cleans transactional loan data, handles missing collateral values, evaluates risk distributions, and compares capital requirement outcomes using two primary regulatory methodologies:
1. **The Standardized Approach (SA)**
2. **The Internal Ratings-Based Approach (IRB)**

## 📋 Regulatory Requirements & Data Constraints
- **Regulatory Framework:** Basel III Implementation Standards.
- **Asset Class Focus:** 100% Mortgage Loans.
- **Data Cleansing Protocol:** Implemented a fixed regulatory proxy defaulting missing collateral data lines to a baseline Loan-to-Value **(LTV) ratio of 0.45**.
- **Core Database Metrics Analyzed:**
  - `BAD`: Binary loan status indicator (1 = Defaulted/Delinquent, 0 = Paid).
  - `MORTDUE` / `VALUE`: Outstanding mortgage balances versus total property valuation metrics.
  - `DEROG` / `DELINQ`: Frequency of major derogatory reports and delinquent credit lines.
  - `DEBTINC`: Consumer debt-to-income leverage metrics.
  - `YOJ` / `JOB`: Professional stability parameters (Years at present job and occupational categories).
  - `CLAGE` / `CLNO` / `NINQ`: Historical credit account ages, volumes, and recent inquiry velocities.

## 🛠️ Technical Pipeline & Implementation
- **Data Ingestion & Cleaning:** Python (Pandas) script execution and spreadsheet architectures to audit structural columns.
- **Risk Parameter Modeling:** Execution of probability of default (PD) calculations and data handling protocols.
- **Data Visualization:** Built interactive dashboards (Tableau/Looker Studio) to clearly communicate asset risk concentrations and portfolio distributions.

## 🎯 Portfolio Evaluation Metrics Met
To pass structural institutional audits, this repository explicitly adheres to these core evaluation pillars:
1. **Parameter Identification:** Exact matching of database features to target risk calculation parameters.
2. **Calculation Accuracy:** Rigorous statistical logic applied to cross-compare SA vs. IRB frameworks.
3. **Data Communication:** Clean visual signaling highlighting peak asset default exposures and portfolio vulnerability clusters.
4. **Structured Documentation:** Fully documented reasoning and justification for each data cleaning and analysis choice.

## 🚀 How to Navigate This Repository
- `/data`: Contains references to the mortgage tracking inputs.
- `/scripts`: Houses the core mathematical calculation sheets and optimization models.
- `/visualizations`: Links to the interactive risk parameter dashboards.


Please, look at the fixed file only, and ignore the first one. I did some changes to this project, and the link to this project is in the Colab notebook: https://colab.research.google.com/drive/1ZtVmUuuFSeCTjdCBGDctxIyqRE2vZQo8#scrollTo=b-tiSpAyfs3I

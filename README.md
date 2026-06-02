# Mortgage Credit Risk & Basel III RWA Analysis

##  Project Overview & Business Goal
This project focuses on calculating Credit Risk Risk-Weighted Assets (RWA) and baseline capital requirements for a bank's mortgage portfolio under the **Basel III Regulatory Framework**. 

The strategic goal is to build an analytical data pipeline that cleans transactional loan data, handles missing collateral values, evaluates risk distributions, and compares capital requirement outcomes using two primary regulatory methodologies:
1. **The Standardized Approach (SA)**
2. **The Internal Ratings-Based Approach (IRB)**

## Regulatory Requirements & Data Constraints
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

## Technical Pipeline & Implementation
- **Data Ingestion & Cleaning:** Python (Pandas) script execution and spreadsheet architectures to audit structural columns.
- **Risk Parameter Modeling:** Execution of probability of default (PD) calculations and data handling protocols.



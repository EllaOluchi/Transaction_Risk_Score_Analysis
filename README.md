# Fraud Detection Analysis – 947 Customers, 5 Countries  

## Project Objective  
The objective of this project is to analyze **customer transactions across five countries** (China, Nigeria, Pakistan, Russia, and Venezuela) in order to detect fraud risks, identify suspicious behaviors, and highlight systemic vulnerabilities.  

**Focus Areas:**  
- Identifying high-risk customers with past fraud history.  
- Detecting customers with unusual multi-country activity.  
- Analyzing transaction amounts for outliers and fraud-prone thresholds.  
- Highlighting high-risk transaction types (Wire Transfers & ATM Withdrawals).  
- Comparing countries by fraud risk, anomaly scores, and flagged customers.  
- Assessing correlation between transaction amounts and fraud indicators.  

**In short:** This project uncovers fraud-prone customers, risky locations, and weak transaction controls.  

## Files in this Repository  
- `Transaction Risk Scoring Report.xlsx` → Full dataset, analysis, and dashboards.  
- `REPORT.md` → Detailed insights and recommendations.  
- `README.md` → Project overview (this file).  

## Overview of Dataset  
- **947 customers**  
- **5 countries** (China, Nigeria, Pakistan, Russia, Venezuela)  
- **1,000 transactions**  
- **2,536,377.59** in total value  

## Key Insights (Summary)  
- **147 customers** previously flagged for fraud.  
- **39 customers** transacted across multiple countries.  
- Transactions **above 4,718.90** strongly linked to fraud (65 cases).  
- **Wire Transfers & ATM Withdrawals** → highest fraud risk.  
- **Venezuela** → most fraud-prone location.  
- **Nigeria** → lowest relative risk, but still high-value anomalies.  
- Strong correlation between **transaction amount and fraud risk**.  

## Recommendations (Summary)  
- Strengthen controls for **Wire Transfers & ATM Withdrawals** (biometrics, real-time alerts).  
- Stricter monitoring in **Venezuela & Nigeria** (threshold alerts, blacklist offenders).  
- Investigate **147 flagged customers** and the **39 multi-country customers**.  
- Enforce stricter **cross-border verification** and KYC reinvestigation.

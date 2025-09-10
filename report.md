# Detailed Report – Transaction Risk Score Analysis  

## Overview Analysis  
- **947 customers**  
- **5 countries**: China, Nigeria, Pakistan, Russia, Venezuela  
- **1,000 transactions**  
- **2,536,377.59** in total value  


## INSIGHTS  

### 1. Customer Based Analysis  
- **147 customers (16%)** previously flagged for fraud.  
- **39 customers** carried out transactions in multiple countries.  

**Multi-country Customers (No previous fraud history):**
| No Previous History of Fraud | Previous History of Fraud |
|------------------------------|---------------------------|
| CUST9666                     | CUST7949                  |
| CUST7938                     | CUST6486                  |
| CUST6977                     | CUST4627                  |
| CUST6592                     | CUST3327                  |
| CUST8392                     | CUST4170                  |
| CUST7287                     | CUST2184                  |
| CUST9120                     | CUST5780                  |
| CUST8400                     | CUST2062                  |
| CUST2693                     | CUST9905                  |
| CUST8560                     | CUST7941                  |
| CUST5146                     | CUST4072                  |
| CUST1876                     | CUST4486                  |
| CUST6732                     | CUST2531                  |
| CUST5380                     | CUST7316                  |
| CUST8186                     | CUST4719                  |
| CUST8266                     | CUST1009                  |
| CUST6588                     | CUST2460                  |
| CUST4636                     | CUST3048                  |
| CUST9702                     | CUST3832                  |
|                              | CUST2906                  |


### 2. Transaction Amount Analysis  
- Transactions **above $4,718.90** (upper 1.5 std dev):  
  - 65 transactions (6.5% of total).  
  - **83% are Medium Risk.**  
- Transactions **below $353.86** (lower 1.5 std dev):  
  - 65 transactions (6.5% of total).  
  - **92% are Low Risk.**  
- **95th percentile = $4,779.87** → only 5% of transactions exceed this.  


### 3. Transaction Type Analysis  
- **Wire Transfers & ATM Withdrawals** = highest anomaly scores and fraud likelihood.  
- Wire Transfers account for **31% (20 cases)** of transactions above $4,718.90.  


### 4. Location Based Analysis  
- **Venezuela**: Highest fraud risk (avg. risk score, anomaly, likelihood).  
- **33 Venezuelan customers** already flagged for fraud.  
- **Nigeria**: Lowest relative risk, but **15 transactions above $4,718.90 (23.1%)**.  


### 5. Correlation Analysis  
- Transaction amount is positively correlated with:  
  - Risk Score  
  - Anomaly Score  
  - Fraud Likelihood %  
- These three fraud indicators also correlate with each other → higher amounts = higher fraud likelihood.  


## RECOMMENDATIONS  

1. **Strengthen Security for Wire Transfers & ATM Withdrawals**  
   - Introduce biometrics for high-value transactions.  
   - Enable real-time alerts.  
   - Use dynamic thresholds for amounts above **$4,718.90**.  

2. **Higher Monitoring in Venezuela & Nigeria**  
   - Apply stricter thresholds for Venezuela.  
   - Use machine learning to detect country-specific fraud.  
   - Transaction alerts for Nigeria’s high-value cases.  
   - Blacklist repeat offenders.  

3. **Investigate Flagged and Multi-country Customers**  
   - Re-check the **147 previously flagged customers**.  
   - Investigate **39 multi-country customers** for possible account sharing or proxy activity.  
   - Conduct fresh KYC verification.  

4. **Cross-border Transaction Controls**  
   - Require additional verification for cross-country transfers.  
   - Monitor customer travel behavior to validate multi-location activity.

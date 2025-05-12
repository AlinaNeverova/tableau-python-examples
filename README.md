# Tableau Dashboard: Python-Based Correlation & Normality Analysis

This repository contains a Tableau workbook (`.twbx`) that demonstrates the integration of Python (via TabPy) into Tableau for statistical analysis.

## 🔍 Overview

The dashboard showcases how Python scripts can be used directly within Tableau to perform:

1. **Normality Testing**  
   - Method: Anderson-Darling test  
   - Function: `scipy.stats.anderson()`  
   - Purpose: To evaluate whether the distribution of `Affiliate Marketing` data follows a normal distribution.

2. **Correlation Analysis**  
   - Method: Spearman’s Rank Correlation  
   - Function: `scipy.stats.spearmanr()`  
   - Outputs:
     - Spearman correlation coefficient
     - P-value for significance testing  
   - Purpose: To measure the strength and direction of association between Sales and Marketing Costs.

## 🛠️ Requirements

To fully utilize this dashboard, you need:

- **Tableau Desktop** (non-Public edition)
- **TabPy** (Tableau Python Server Extention)

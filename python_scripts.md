# Python Scripts Used in Tableau (via TabPy)

This document contains a few Python scripts embedded in the uploaded Tableau workbook as examples. 
These scripts were used to perform statistical analysis directly within Tableau visualizations.

## 1. Normality Test (Anderson-Darling)

**Script:**

SCRIPT_REAL("
import scipy.stats
return [scipy.stats.anderson(_arg1, dist='norm').statistic]
",
SUM([Affiliate Marketing])
)


## 2. Spearman Correlation Coefficient

**Script:**

SCRIPT_REAL("
import scipy.stats
return scipy.stats.spearmanr(_arg1, _arg2)[0]
",
SUM([Product Sold]), SUM([Affiliate Marketing])
)


## 3. P-value for Correlation Significance

**Script:**

SCRIPT_REAL("
import scipy.stats
return scipy.stats.spearmanr(_arg1, _arg2)[1]
",
SUM([Product Sold]), SUM([Affiliate Marketing])
)

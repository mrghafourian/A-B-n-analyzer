# abnalyzer

A Python tool for analyzing A/B(/n) tests with conversion rate significance and revenue metrics.  
Runs easily in Jupyter Notebook.

## Features
- Handles A/B/n experiments
- Conversion rate, lift, p-values, confidence intervals
- Multiple comparison correction (Holm/Bonferroni/BH-FDR)
- Revenue metrics: AOV, RPV
- Export results to CSV/Excel

## Quick Start
```python
from abcalc_notebook import analyze_file

pretty, raw = analyze_file("sample_data/ab_test_with_revenue.csv")

# abnalyzer

A Python tool for analyzing A/B(/n) tests with conversion rate significance and revenue metrics.  
Runs easily in Jupyter Notebook.

## Features
- Handles A/B/n experiments
- Conversion rate, lift, p-values, confidence intervals
- Multiple comparison correction (Holm/Bonferroni/BH-FDR)
- Revenue metrics: AOV, RPV
- Export results to CSV/Excel
- Easy to run in Jupyter
---

## 📂 Example Input
CSV file:
```csv
variant,visits,conversions,revenue
A,10074,772,36133
B,10234,824,38108
C,10478,915,41481
D,10362,720,34045

## Quick Start
```python
from abcalc_notebook import analyze_file

pretty, raw = analyze_file("sample_data/ab_test_with_revenue.csv")

# abnalyzer

A Python tool for analyzing A/B(/n) tests with conversion rate significance and revenue metrics.  
Runs easily in Jupyter Notebook.

## Features
- Handles A/B/n experiments
- Conversion rate, lift, p-values, confidence intervals
- Multiple comparison correction (Holm/Bonferroni/BH-FDR)
- Revenue metrics: AOV, RPV
- Export results to CSV/Excel

## 🌍 Real-World Applications

This tool is useful anywhere A/B(/n) testing is applied to make data-driven decisions, such as:

- **Marketing campaigns** → test email subject lines, ad creatives, or CTAs.  
- **Web & UX design** → compare landing pages, checkout flows, or navigation menus.  
- **E-commerce & pricing** → evaluate offers (Free Shipping vs 10% Off) or price points.  
- **SaaS & product features** → analyze onboarding flows, upsells, or new features.  

It helps answer the key question: *“Is the observed difference real, or just random noise?”*  

## Example Input
CSV file:
```csv```

variant,visits,conversions,revenue

A,10074,772,36133

B,10234,824,38108

C,10478,915,41481

D,10362,720,34045

## Quick Start
```python```
from abcalc_notebook import analyze_file

pretty, raw = analyze_file("sample_data/ab_test_with_revenue.csv")

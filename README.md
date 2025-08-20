# Email Campaign A/B Testing

## Overview
This project analyzes an **A/B test on email campaigns** to determine whether a **new landing page (treatment)** improves the conversion rate compared to the **old landing page (control)**. The analysis includes **data cleaning, visualization, hypothesis testing, and confidence interval estimation** to make data-driven recommendations.

## Goal
- Compare conversion rates between the old landing page (control) and the new landing page (treatment).
- Evaluate whether the new landing page leads to a statistically significant improvement in conversions.

## Tools & Libraries
- **Python**
- **pandas** – Data manipulation
- **numpy** – Numerical operations
- **matplotlib** – Data visualization
- **statsmodels** – Statistical testing

## Dataset
- Dataset: `ab_data.csv`
- Contains:
  - `user_id` – Unique identifier for each user
  - `group` – Assigned group (control/treatment)
  - `landing_page` – Page shown to the user (old/new)
  - `converted` – Conversion flag (0 = no, 1 = yes)
  - `timestamp`  – Timestamp of the user's visit

## Steps Performed
1. **Data Cleaning**
   - Removed mismatched group/landing page pairs.
   - Dropped duplicate users to ensure data integrity.
2. **Exploratory Analysis**
   - Checked group sizes and unique conversion values.
   - Calculated conversion rates for control and treatment groups.
   - Visualized conversion rates using bar plots.
3. **Statistical Testing**
   - Conducted **Z-test** for proportions to determine statistical significance.
   - Calculated **95% confidence intervals** for both groups.
   - Visualized conversion rates with error bars.
4. **Trend Analysis**
   - Plotted **daily conversion trends** using timestamp data.
5. **Conclusion & Recommendations**
   - Absolute difference between conversion rates calculated.
   - Statistical significance interpreted.
   - Suggestions for next steps and potential improvements.

## Key Findings
- Conversion Rates:
  - Control (old page): **12.04%**
  - Treatment (new page): **11.88%**
  - Absolute difference (B − A): **−0.158 percentage points**
- **Statistical Significance:** Not significant (p-value = 0.1899 > 0.05)
- 95% Confidence Intervals overlap, indicating observed differences may be due to random variation.
- **Recommendation:** No immediate rollout of the new page. Consider testing more variants or segmenting users for targeted improvements.

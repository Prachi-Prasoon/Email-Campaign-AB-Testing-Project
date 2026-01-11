# Email Campaign A/B Testing – Business Analytics Project

## Overview
This project presents an end-to-end A/B testing analysis conducted on an
email marketing campaign to evaluate whether a new landing page improves
user conversion rates compared to an existing landing page.

The project demonstrates how experimental data can be transformed into
clear business recommendations using statistical analysis and analytical
best practices.

---

## Business Problem
Despite strong user acquisition through email campaigns, conversion rates
remained stagnant. The marketing team introduced a redesigned landing page
and ran an A/B experiment to assess whether the new experience drives
higher conversions.

The key question addressed in this project is:
**Should the new landing page be rolled out to all users?**

---

## Dataset
The analysis uses an event-level dataset containing:
- `user_id`: Unique user identifier
- `group`: Experiment group (control or treatment)
- `landing_page`: Page shown to the user
- `converted`: Conversion indicator (0 or 1)
- `timestamp`: Time of user interaction

Total users analyzed: **290,584**

---

## Tools & Technologies
- Python
- pandas
- numpy
- matplotlib
- statsmodels
- Jupyter Notebook

---

## Analysis Approach

The project follows a structured, industry-standard experimentation workflow:

1. **Data Cleaning**
   - Removed mismatched group and landing page records
   - Deduplicated users to ensure one observation per user

2. **Experiment Validation**
   - Sanity checks on group sizes and conversion values
   - Sample Ratio Mismatch (SRM) testing to validate randomization

3. **Conversion Analysis**
   - Computed conversion rates for control and treatment groups
   - Estimated absolute and relative differences

4. **Statistical Testing**
   - Conducted two-sample Z-test for proportions
   - Evaluated statistical significance at a 5% level
   - Calculated 95% confidence intervals

5. **Power Analysis**
   - Assessed whether the experiment was sufficiently powered
   - Evaluated sensitivity to detect a 1% absolute lift

6. **Time Trend Analysis**
   - Analyzed daily conversion rates to identify temporal bias

7. **Business Impact Estimation**
   - Translated conversion differences into estimated revenue impact

---

## Key Findings
- The new landing page resulted in a slightly lower conversion rate than the old page
- The observed difference was not statistically significant
- Confidence intervals overlapped across variants
- The experiment was sufficiently powered
- Rolling out the new page introduces potential downside risk without
  measurable upside

---

## Final Recommendation
The analysis does not support rolling out the new landing page.

Instead, it is recommended to:
- Test alternative page designs or messaging
- Run segmented experiments to identify user-specific effects
- Clearly define minimum detectable effects for future experiments

---

## Project Structure

Email-Campaign-AB-Testing/
│
├── data/
│ └── ab_data.csv
│
├── notebooks/
│ └── ab_testing.ipynb
│
├── reports/
│ └── experiment_summary.md
│
├── visuals/
│ └── conversion_rates.png
│ └── daily_trends.png
│
└── requirements.txt


---

## What This Project Demonstrates
- Strong understanding of experiment design and validation
- Ability to apply statistical testing to real business problems
- Focus on decision-making, not just statistical significance
- Translation of analytical results into business impact
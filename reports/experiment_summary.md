# Email Campaign A/B Test – Experiment Summary

## Objective
The objective of this experiment was to evaluate whether a new landing page
improves conversion rates for an email marketing campaign compared to the
existing landing page.

The outcome of this analysis was intended to support a data-driven rollout
decision for the marketing team.

---

## Experiment Overview
- Total users analyzed: 290,584
- Control group: Old landing page (145,274 users)
- Treatment group: New landing page (145,310 users)
- Metric: Conversion Rate (binary conversion indicator)
- Unit of randomization: User
- Significance level: 5%

Users were randomly assigned to either the control or treatment group and
exposed to the corresponding landing page.

---

## Data Validation & Experiment Integrity
Several checks were performed to ensure experiment validity:

- Mismatched group and landing page records were removed
- Duplicate users were deduplicated
- Conversion values were verified to be binary
- Sample Ratio Mismatch (SRM) testing showed no evidence of biased traffic
  allocation (p-value > 0.01)

These checks confirm that the experiment setup and randomization were valid.

---

## Key Results

### Conversion Rates
- Control (old page): 12.04%
- Treatment (new page): 11.88%
- Absolute difference: -0.16 percentage points

### Statistical Significance
- Z-statistic: 1.31
- P-value: 0.1899

At a 5% significance level, the observed difference is not statistically
significant. The null hypothesis cannot be rejected.

### Confidence Intervals (95%)
- Control: 11.87% – 12.21%
- Treatment: 11.72% – 12.05%

The overlap between confidence intervals further suggests that the observed
difference may be due to random variation.

---

## Power Analysis
The experiment was evaluated to detect a minimum detectable effect (MDE) of
1% absolute lift with 80% statistical power and a 5% significance level.

- Required sample size per group: ~2,275 users
- Actual sample size per group: ~145,000 users

The experiment was sufficiently powered to detect a 1% or greater change in
conversion rate. Smaller effects, if present, were not the target of this test.

---

## Time Trend Analysis
Daily conversion rates were analyzed over the experiment period. No consistent
or sustained divergence was observed between the control and treatment groups
over time.

This indicates stable experiment behavior without temporal bias.

---

## Business Impact Estimation
While the conversion difference is small, at scale it can have material
financial implications.

Using estimated monthly traffic and average order value:
- Rolling out the new landing page could potentially reduce monthly revenue
- This introduces unnecessary downside risk without clear performance gains

---

## Final Recommendation
Based on statistical evidence and business impact considerations:

- Do **not** roll out the new landing page
- Continue experimentation with alternative designs or messaging
- Define clear minimum detectable effects prior to future tests
- Consider segmented experiments (e.g., device type or traffic source)

The current experiment does not provide sufficient evidence that the new
landing page improves conversion performance.
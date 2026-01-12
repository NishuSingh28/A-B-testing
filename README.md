# A/B Testing Analysis – Landing Page Experiment

## Overview
End-to-end A/B testing analysis of an e-commerce landing page experiment using frequentist and Bayesian methods.

- Dataset: 290,584 users (~145K per group)
- Primary metric: Conversion rate
- Final decision: Do not ship the new page

---

## Key Results

| Analysis | Outcome |
|--------|--------|
| Observed effect | −0.16 percentage points (−1.33% relative) |
| Frequentist test | p = 0.184 (not significant) |
| Bayesian analysis | 91% probability control performs better |
| Power analysis | 26% power for observed effect |
| Segment analysis | No significant segments after correction |

---

## Final Recommendation
Do not ship the new landing page.

**Rationale**
- No statistically significant improvement
- High probability that control performs better
- Effect size is small and unstable
- Expected loss from shipping treatment is higher than keeping control

---

## What This Project Demonstrates
- Complete A/B testing workflow (design, validation, analysis, decision)
- Frequentist methods (z-test, confidence intervals, power)
- Bayesian inference (Beta–Binomial model, sensitivity analysis)
- Data quality checks (assignment–exposure mismatch)
- Segment and temporal stability analysis
- Multiple testing correction (Benjamini–Hochberg)

---

## Methods and Tools

**Statistics**
- Two-proportion z-test
- Bayesian A/B testing (PyMC)
- Power analysis
- Multiple testing correction

**Tech stack**
Python, Pandas, NumPy, SciPy, PyMC, ArviZ, Statsmodels, Matplotlib

---

## Files
- `ab_testing_analysis.ipynb` – Complete analysis
- `NOTEBOOK_SUMMARY.md` – Final conclusions and decision summary

---

## References
- Frequentist A/B Testing: https://ethen8181.github.io/machine-learning/ab_tests/frequentist_ab_test.html
- Bayesian A/B Testing (PyMC): https://www.pymc.io/projects/examples/en/latest/causal_inference/bayesian_ab_testing_introduction.html

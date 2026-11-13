# Dataset Structure & 95% Confidence Level Methodology

## 1. Dataset Overview (Primary & Secondary Integration)
To evaluate target customer preferences without relying solely on broad industry assumptions, a combined dataset was constructed:
* **Primary Dataset:** Structured survey responses capturing customer preferences, feature priorities, price sensitivity, and brand perception across target cohorts.
* **Secondary Dataset:** Triangulated benchmarks from industry reports, market sizing studies, and competitor customer reviews to validate baseline trends.
* **Data Hygiene & Preparation:** Removed incomplete responses, standardized categorical preference scales, and checked for demographic/cohort skew before running statistical validation.

---

## 2. How the 95% Confidence Level Was Achieved
To ensure that observed customer preference trends were statistically reliable rather than random sampling noise, the sample size and margin of error were validated using standard confidence interval estimation:

### Statistical Parameters
* **Confidence Level ($1 - \alpha$):** **95%** (corresponding to a critical Z-score of **$Z = 1.96$**)
* **Margin of Error ($E$):** **$\pm 5\%$** ($0.05$)
* **Population Proportion ($p$):** **$0.5$** (conservative maximum-variability assumption)

### Sample Size & Confidence Interval Formula
$$n = \frac{Z^2 \cdot p \cdot (1 - p)}{E^2}$$

Substituting the parameters:
$$n = \frac{(1.96)^2 \cdot 0.5 \cdot (1 - 0.5)}{(0.05)^2} = \frac{3.8416 \cdot 0.25}{0.0025} \approx 385 \text{ validated responses}$$

### Confidence Interval Validation for Preference Metrics
For each key customer preference proportion ($\hat{p}$), the confidence interval was verified using:
$$\text{CI} = \hat{p} \pm Z \sqrt{\frac{\hat{p}(1 - \hat{p})}{n}}$$

## 3. Key Analytical Takeaways from the Dataset
* **Statistically Significant Preferences:** Core customer pain points and feature preferences cleared the 95% confidence threshold, eliminating guesswork in segment prioritization.
* **Cross-Validation:** Primary survey findings aligned closely with secondary industry benchmarks, confirming external validity.

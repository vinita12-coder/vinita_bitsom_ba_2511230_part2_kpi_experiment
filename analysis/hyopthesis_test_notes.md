# Hypothesis Test Notes

## Objective
The purpose of this analysis is to assess whether the new onboarding campaign (Treatment Group) performs meaningfully better than the existing onboarding experience (Control Group) in driving Paid Conversion Rate improvements.

The outcome of this hypothesis test informs the business decision on whether to proceed with rolling out the new onboarding experience.

---

# Hypothesis

## Null Hypothesis (H₀)
There is **no statistically significant difference** between the Paid Conversion Rate of the Control Group and the Treatment Group.

[
H_0 : p_{Control} = p_{Treatment}
]

---

## Alternative Hypothesis (H₁)
There is a **statistically significant difference** between the Paid Conversion Rate of the Control Group and the Treatment Group.

[
H_1 : p_{Control} \neq p_{Treatment}
]

---

# Test Configuration

| Item                   | Value                                 |
| ---------------------- | ------------------------------------- |
| Primary Metric         | Paid Conversion Rate                  |
| Test Type              | Two-Sample t-Test (Unequal Variances) |
| Tail Type              | Two-Tailed                            |
| Significance Level (α) | 0.05                                  |

---

# Reason for Selecting the Metric
Paid Conversion Rate was chosen as the primary evaluation metric because it directly reflects the proportion of users who become paying subscribers. Driving this metric upward contributes directly to subscription growth and overall business revenue, making it the most relevant measure of onboarding campaign success.

---

# Hypothesis Test Results

## Test Inputs

| Metric               |  Value |
| -------------------- | -----: |
| Control Group Size   |    693 |
| Treatment Group Size |    715 |
| Mean (Control)       | 0.0317 |
| Mean (Treatment)     | 0.0699 |

---

## Statistical Output

| Metric             |  Result |
| ------------------ | ------: |
| t Statistic        | -3.2801 |
| Two-Tailed P-value |  0.0011 |
| Alpha              |    0.05 |

---

# Decision Rule

* If **P-value < 0.05**, reject the Null Hypothesis.
* If **P-value ≥ 0.05**, fail to reject the Null Hypothesis.

Since the **P-value (0.0011)** falls below the significance level of **0.05**, the Null Hypothesis is rejected.

---

# Business Interpretation
The statistical results indicate that the Treatment Group achieved a substantially higher Paid Conversion Rate than the Control Group. The observed difference is unlikely to be explained by random variation and provides strong evidence that the redesigned onboarding campaign outperforms the existing experience.

---

# Guardrail Metrics Evaluation
While the Treatment Group improved the primary business metric, a set of guardrail metrics was also reviewed before forming a recommendation.

| Guardrail Metric                   | Observation                        | Risk Assessment |
| ---------------------------------- | ---------------------------------- | --------------- |
| Refund Rate                        | Increased slightly (0.00% → 0.42%) | Low Risk        |
| Support Ticket Rate                | Increased (14.72% → 24.76%)        | Medium Risk     |
| Average Days to Convert            | Reduced (8.86 → 6.40 days)         | Positive        |
| Average Engagement Score           | Improved (57.03 → 62.93)           | Positive        |
| Average Revenue per Converted User | Declined (1630.10 → 770.41)        | Medium Risk     |

---

# Guardrail Interpretation
The Treatment Group converted users more quickly and showed stronger customer engagement, both of which are favourable indicators for business growth. However, the rise in support ticket volume and the decline in average revenue per converted user highlight areas that will need ongoing attention following deployment.

Overall, none of the guardrail metrics present a critical business risk sufficient to block the rollout of the new onboarding experience.

---

# Final Conclusion
Based on the statistical evidence and KPI evaluation:

* Paid Conversion Rate improved significantly under the Treatment experience.
* The Null Hypothesis was rejected.
* The Treatment Group outperformed the Control Group on the primary metric.
* Guardrail risks remain at a manageable level.

The analysis therefore supports recommending the new onboarding campaign for full business rollout, with continued monitoring of key guardrail metrics following launch.

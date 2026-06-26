# KPI Framework, Business Experiment Analysis & Decision Recommendation

## Project Overview
This project evaluates the effectiveness of a redesigned onboarding campaign for a subscription-based digital product using A/B testing. The objective is to determine whether the new onboarding experience should replace the current process, based on statistical evidence, KPI performance, and business risk assessment.

---

## Business Problem
The company launched a redesigned onboarding experience aimed at improving early user activation and paid subscription conversion. Users were randomly allocated to either the Control Group (existing onboarding) or the Treatment Group (new onboarding). The business needs to decide whether the new experience should be rolled out to all users.

This decision has direct implications for product managers, marketing teams, and business leadership. The primary goal is to improve the Paid Conversion Rate without negatively affecting customer experience or overall business quality.

---

## North Star Metric

**Paid Conversion Rate**

This metric directly measures the proportion of users who become paying subscribers and therefore serves as the primary indicator of business growth.

**Supporting KPIs include:**

* Landing Page Visit Rate
* Trial Start Rate
* Onboarding Completion Rate
* Average Engagement Score
* Average Revenue per User

**Guardrail metrics include:**

* Refund Rate
* Support Ticket Rate
* Average Revenue per Converted User
* Average Days to Convert

---

## KPI Tree
The KPI Tree is anchored by the North Star Metric (Paid Conversion Rate) and structured around three primary drivers:

* User Acquisition & Activation
* User Engagement
* Revenue Quality

Each driver is supported by relevant sub-drivers, while guardrail metrics ensure that business quality is preserved throughout the optimisation process.

---

## Data Preparation
The dataset was thoroughly reviewed prior to analysis.

**Validation checks performed:**

* Missing values reviewed and documented
* Duplicate User IDs identified and recorded
* Binary field values validated
* Group balance verified across Control and Treatment
* Revenue outliers examined
* Segment distribution assessed

No critical data quality issues were found that would prevent further analysis from proceeding.

---

## Repository Structure

```text
part2_kpi_experiment/
├── data/
│   └── campaign_experiment_data.xlsx
├── analysis/
│   ├── experiment_analysis.xlsx
│   └── hypothesis_test_notes.md
├── outputs/
│   ├── kpi_tree.png
│   ├── experiment_summary.xlsx
│   └── recommendation_memo.md
├── screenshots/
│   ├── summary_metrics.png
│   ├── hypothesis_test_output.png
│   └── kpi_tree_preview.png
└── README.md
```

---

## Tools Used

* Microsoft Excel
* Pivot Tables
* Excel Formulas
* Two-Sample t-Test
* KPI Framework
* Markdown

---

## Conclusion
The statistical analysis and KPI evaluation indicate that the new onboarding campaign meaningfully improves paid user conversion while keeping business risk at an acceptable level. The Treatment Group demonstrates stronger overall performance and is recommended for full rollout, with ongoing monitoring of guardrail metrics advised post-launch.

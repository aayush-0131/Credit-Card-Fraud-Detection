# Credit Card Fraud Detection and Cost Optimization

A statistical-optimization **course team project** on the asymmetric costs of false-positive and false-negative fraud classifications.

## Project and contribution attribution

This work was prepared by three team members, as documented in the committed Quarto report:

| Team member | Contribution recorded in the report |
| --- | --- |
| Aayush Jha (BSDCC2401) | Led formulation of the optimization problem and helped implement the gradient-descent solution |
| Amartya Amritanshu (BSDCC2405) | Data preprocessing, visualization and contributions to LP/QP formulation |
| Paduri Sanjith Reddy (VSDCC2412) | Cost-model design, sensitivity analysis and presentation slides |

These are the contributions **reported by the team**. Repository ownership should not be interpreted as sole authorship or as proof that every described component was written by one person.

## Research question

Can credit-card fraud classification be formulated to minimize expected misclassification cost, rather than optimizing accuracy alone? The report discusses cost-sensitive logistic regression, linear programming and quadratic programming approaches, using a public, highly imbalanced transaction dataset.

## Available artifacts

- [Written team report (PDF)](12-jha-amritanshu-reddy-project-report.pdf)
- [Editable report source (Quarto)](12-jha-amritanshu-reddy.qmd)
- [Team presentation](12-jha-amritanshu-reddy_presentation.pptx)

## Evidence and reproducibility limits

The report describes a roughly 35% reduction in average cost per transaction compared with its baseline, along with other performance claims. **Those claims have not been independently reproduced in this repository.** The report refers to preprocessing, optimization and results notebooks in a separately submitted ZIP, but those notebooks are not currently committed here. This repository currently contains a report and presentation, **not a complete runnable end-to-end experiment**.

There is also a methodological detail to verify before promoting results: the report mentions SMOTE and an 80/20 train-test split without sufficiently establishing their precise order or the pipeline used for held-out evaluation. Leakage-safe resampling must be confirmed from the original code rather than assumed.

Until the missing code and evaluation protocol are reviewed, treat numerical results as **reported team findings**, not independently verified portfolio-performance claims.

## Scope

This repository preserves academic team work and the documented research question. It does not establish a deployed fraud-detection service, bank/customer impact, or production risk reduction.

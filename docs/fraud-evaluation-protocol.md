Fraud Detection Evaluation Protocol

Status: Draft v0.1

Purpose

Define a fair, reproducible evaluation protocol for candidate fraud-risk models.

Evaluation metrics

- Precision: proportion of flagged cases that are confirmed positive.
- Recall: proportion of confirmed positive cases detected.
- F1 score: harmonic mean of precision and recall.
- False-positive rate: proportion of negative cases incorrectly flagged.
- Precision-recall curve: trade-off between precision and recall across thresholds.

Experimental controls

Use a documented baseline and separate training, validation, and test data. Prevent leakage of post-outcome information. Document class imbalance, label quality, and the timing of available features.

Human review

A model flag is an indicator for investigation, not proof of fraud. Document review procedures, appeal pathways, and the consequences of false accusations.

Acceptance criteria

- [ ] Baseline and metrics are defined.
- [ ] Dataset splitting and leakage controls are documented.
- [ ] Threshold selection has a stated rationale.
- [ ] False-positive and false-negative consequences are discussed.
- [ ] No performance claims are made without test results.

Next action

Create a synthetic labeled dataset and implement a simple baseline evaluation before testing more complex models.
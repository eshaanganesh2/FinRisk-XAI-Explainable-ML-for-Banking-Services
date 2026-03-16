# Banking Services Prediction with Explainable AI

An ensemble machine learning system that models three sequential banking decisions: customer churn, credit default risk, and loan repayment eligibility using a 
cascaded architecture where each model's output gates the next. SHAP analysis is 
applied across all three models to produce interpretable, feature-level explanations 
for each prediction.

Published and presented at the International Conference for Contemporary 
Computing (IC3) 2022 — https://doi.org/10.1145/3549206.3549259

## Models

**1. Customer Satisfaction / Churn Prediction**
Classifies whether a customer is likely to churn based on behavioral signals 
(credit score, product ownership, service utilization frequency). A churn prediction 
triggers the credit default pipeline.

**2. Credit Default Prediction**
Evaluates six months of credit card statement history to assess whether an 
at-risk customer is still creditworthy, informing retention offer decisions.

**3. Loan Repayment Prediction**
Independently assesses loan eligibility using customer demographics and loan 
parameters (intent, amount, interest rate, employment length).

## Explainability
SHAP (SHapley Additive Explanations) analysis is applied to each model to quantify 
per-feature contribution, providing directional and magnitude-level insight into 
model decisions, critical for auditability in regulated financial contexts.

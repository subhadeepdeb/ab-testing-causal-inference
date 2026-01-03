# A/B Testing & Causal Inference — Product Experiment

## Problem
Evaluate whether a new product onboarding flow improves user conversion and revenue using a randomized A/B experiment.

## Experiment Design
- **Control:** Existing onboarding flow
- **Treatment:** New onboarding flow
- **Primary Metric:** Conversion rate
- **Secondary Metric:** Revenue per user (RPU)

Users are randomly assigned to control and treatment groups, enabling causal interpretation of results.

## Data
- Synthetic but realistic experiment dataset
- ~10,000 users split evenly between control and treatment
- Variables include group assignment, conversion outcome, and revenue

## Methodology
- Sanity checks and metric validation
- Proportion z-test for conversion rate
- Welch’s t-test for revenue comparison
- Difference-in-means estimation for causal effect (ATE)
- Bootstrap confidence intervals for robustness

## Results
- Treatment group shows higher conversion rate than control
- Revenue per user also increases under treatment
- Effects are statistically significant and practically meaningful

## Causal Interpretation
Because treatment assignment is randomized, the difference in average outcomes between groups provides an unbiased estimate of the **Average Treatment Effect (ATE)**.

## Recommendation
Roll out the new onboarding flow, while continuing to monitor downstream metrics such as retention and customer support load.

## Repository Structure


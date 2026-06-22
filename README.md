# Why-the-Fraud-

# What Characteristics Are Associated with Insurance Fraud?

## Overview

Insurance fraud costs the insurance industry billions of dollars annually and increases premiums for policyholders. This project investigates which claim, policy, financial, and demographic characteristics are associated with fraudulent insurance claims.

Using a dataset of 1,000 vehicle insurance claims, we applied exploratory data analysis and logistic regression modeling in R to identify factors that influence the likelihood of fraud.

## Research Question

**What characteristics are associated with insurance fraud, and which factors are the strongest predictors of fraudulent claims?**

## Dataset

The dataset contains information on:

* Insurance claim outcomes (fraudulent or non-fraudulent)
* Claim characteristics
* Policy details
* Financial variables
* Demographic information

### Key Variables

* `fraud_reported` – Whether a claim was reported as fraudulent
* `incident_severity` – Severity level of the incident
* `total_claim_amount` – Total amount claimed
* `policy_deductible` – Deductible associated with the policy
* `policy_annual_premium` – Annual premium amount
* `umbrella_limit` – Umbrella coverage limit
* `insured_sex` – Policyholder gender
* `insured_education_level` – Education level
* `insured_occupation` – Occupation

## Methods

### Exploratory Data Analysis (EDA)

We examined distributions and relationships among variables using:

* Histograms
* Boxplots
* Bar charts
* Summary statistics

### Statistical Modeling

We used logistic regression to model the probability of insurance fraud.

Analyses included:

* Odds ratio interpretation
* Likelihood ratio tests
* Confidence intervals
* Model comparison and diagnostics

## Key Findings

### Strongest Predictor: Incident Severity

Incident severity emerged as the most significant predictor of fraud.

Compared to minor incidents:

* Major damages substantially increased the odds of fraud.
* Total losses were associated with even higher fraud likelihood.

### Limited Impact of Financial Variables

Variables such as:

* Annual premium
* Deductible amount
* Umbrella coverage limit

showed little evidence of independently predicting fraud.

### Claim Amount Alone Was Not Sufficient

While fraudulent claims often involved larger payouts, claim amount by itself was not as informative as incident severity.

## Results

The final logistic regression model suggests that characteristics describing the nature and severity of an incident provide more predictive power than policy structure or financial measures.

These findings highlight the importance of focusing fraud detection efforts on claim context rather than solely on claim size or policyholder financial characteristics.

## Tools & Technologies

* **R**
* **tidyverse**
* **ggplot2**
* **broom**
* **Quarto**
* Logistic Regression
* Statistical Inference


## Authors

* Swikriti Dumre
* Nandir Altansukh
* Hadiya Abdi

## Future Work

Potential extensions include:

* Random Forest and Gradient Boosting models
* Feature engineering for claim characteristics
* Fraud risk scoring systems
* Model performance comparison using ROC and AUC metrics

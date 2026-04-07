# A-B-Test-Analysis-Evaluating-a-New-Feature's-Impact-on-Conversion-Rate

## Overview

This project analyzes the impact of a new product feature on user conversion rate using an A/B testing framework. The goal is to determine whether the feature should be rolled out based on statistical and practical significance.

## Problem

A new feature is introduced to improve user conversion. We want to answer:
Does the feature significantly increase conversion rate, and should it be launched?

## Experiment Design

Population: 10,000 users.

Groups: Randomly assigned to control and treatment.

Metric: Conversion rate (binary outcome).

## Hypothesis

H₀: No difference between groups.

H₁: Treatment increases conversion.

## Data

The dataset was simulated to reflect realistic experimental conditions:

Control conversion rate: 10%

Treatment conversion rate: 12%

Each user is assigned:

group (control/treatment)

conversion outcome (0/1)

## Analysis

Computed conversion rates for both groups. Tested for Sample-Ratio Mismatch. Estimated lift (difference in conversion). Conducted two-proportion z-test. Calculated confidence intervals.

## Results

Control: ~10%

Treatment: ~12%

Lift: +2 percentage points

p-value: < 0.05


## Decision

The treatment shows a statistically significant and practically meaningful improvement in conversion.

Recommendation: Roll out the feature, while monitoring long-term effects.

## Limitations

Simulated data (not real users).

No guardrail metrics (e.g., retention, latency).

No long-term effect measurement.

Assumes perfect randomization.

## Next Steps

Conduct power analysis for experiment sizing.

Analyze heterogeneous treatment effects (by user segment).

Introduce guardrail metrics.

## Tools

Python (Pandas, NumPy, Scipy, statsmodels)

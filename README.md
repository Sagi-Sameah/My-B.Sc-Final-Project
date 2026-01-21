# My-B.Sc-Final-Project

# Price of Abstention in Participatory Budgeting
This project explores a simple but non-trivial question:

Does higher voter participation always lead to better outcomes?

Using simulation on real-world participatory budgeting data, 
I examine how turnout interacts with population diversity and 
how this interaction affects overall voter satisfaction.

## The Idea

Participatory budgeting is often promoted as "the more people participate, the better".
However, higher participation also introduces more diverse — and sometimes conflicting —
preferences.

This project investigates the trade-off between:
- Inclusivity (higher turnout)
- Alignment and satisfaction with selected projects

The key insight:  
Participation improves outcomes in some settings — but can worsen them in others.

## Turnout vs. Satisfaction

![Average satisfaction vs turnout](images/satisfaction_vs_turnout.png)
Across hundreds of real-world budgeting instances, average satisfaction generally increases
with turnout — but not linearly.

At low turnout levels, outcomes are volatile.
At high turnout levels, additional participation often yields diminishing returns.

## When More Participation Hurts

The impact of voter turnout is not uniform across settings.
City-level simulations reveal that the same participation increase
can lead to different — and sometimes opposite — outcomes.

### Warszawa
![Turnout vs Satisfaction – Warszawa](images/satisfaction_comparison_Warszawa_2023.png)

In Warsaw, higher participation generally leads to increased average satisfaction.
The population structure and preference distribution allow additional voters
to reinforce broadly shared priorities.

---

### Lodz
![Turnout vs Satisfaction – Lodz](images/satisfaction_comparison_Lodz_2024.png)

In Lodz, the pattern is different.
As participation increases, average satisfaction can decline,
reflecting higher preference diversity and conflicting project priorities.

The same aggregation mechanism produces contrasting results,
depending on population structure rather than turnout alone.

#
In relatively homogeneous electorates, higher turnout improves satisfaction.
In heterogeneous or fragmented electorates, increased turnout can reduce satisfaction
under simple aggregation rules.

The same voting rule can produce opposite outcomes — depending on population structure.

## What Was Simulated

- Real-world participatory budgeting datasets (588 instances)
- Probabilistic turnout modeling
- Approval-based voting under budget constraints
- Bootstrapped simulations for robustness
- Satisfaction measured at the population level

## Why This Matters

The results challenge the assumption that maximizing participation
is always the right policy goal.

They suggest that:
- Population diversity should be monitored
- One-size-fits-all aggregation rules may fail
- Fairness-oriented or proportional methods may be more appropriate in diverse settings

## Full Research Paper

The complete academic paper (B.Sc. Final Project):

📄 [Price of Abstention in Participatory Budgeting – PDF](Paper/Participatory_Budgeting_Final_Project.pdf)

## Tech Stack

Python · NumPy · pandas · matplotlib  
Simulation · Statistical Analysis · Computational Social Choice


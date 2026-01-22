# Price of Abstention in Participatory Budgeting
This project explores a simple but non-trivial policy question:

Does higher voter participation always lead to better outcomes?

Using simulation on real-world participatory budgeting data, 
the project examines how turnout interacts with population diversity
and how this interaction affects outcome quality and voter satisfaction.

## The Idea

Participatory budgeting is commonly framed as a participation-maximization problem.
However, higher turnout also introduces increased preference diversity
and, in some cases, conflicting priorities.

This project examines the trade-off between:
- Inclusivity (higher turnout)
- Outcome alignment and aggregate satisfaction

The key insight:
Participation can improve outcomes — but its effect depends on
population structure and preference heterogeneity.

## Turnout vs. Satisfaction

![Average satisfaction vs turnout](images/satisfaction_vs_turnout.png)
Across hundreds of real-world budgeting instances, average satisfaction generally increases
with turnout — but not linearly.

At low turnout levels, outcomes are volatile.
At high turnout levels, additional participation often yields diminishing returns,
suggesting limited marginal benefit beyond a certain point.

## When More Participation Hurts

The impact of voter turnout is not uniform across settings.
City-level simulations show that identical increases in participation
can lead to different — and sometimes opposite — outcomes.

### Warszawa
![Turnout vs Satisfaction – Warszawa](images/satisfaction_comparison_Warszawa_2023.png)

In Warsaw, higher participation is associated with increased average satisfaction.
The population structure allows additional voters to reinforce
widely shared preferences, leading to more stable outcomes.

---

### Lodz
![Turnout vs Satisfaction – Lodz](images/satisfaction_comparison_Lodz_2024.png)

In Lodz, the pattern differs.
As participation increases, average satisfaction can decline,
reflecting higher preference diversity and competing project priorities.

Under simple aggregation rules, additional participation amplifies conflict
rather than consensus.

#
These results suggest that turnout alone is an incomplete policy target.

In relatively homogeneous electorates, higher participation tends to improve outcomes.
In heterogeneous or fragmented electorates, increased participation may reduce satisfaction
when simple aggregation rules are used.

Identical voting rules can therefore produce opposite effects,
depending on population structure rather than participation levels alone.

## What Was Simulated

- 588 real-world participatory budgeting instances
- Probabilistic turnout modeling
- Approval-based voting under budget constraints
- Bootstrapped simulations for robustness
- Population-level satisfaction metrics

## Why This Matters

The findings challenge the assumption that maximizing participation
should always be the primary policy objective.

They suggest that:
- Population diversity should be explicitly accounted for
- One-size-fits-all aggregation rules may lead to suboptimal outcomes
- Fairness-oriented or adaptive mechanisms may be more appropriate
  in heterogeneous settings

## Full Research Paper

The complete academic paper (B.Sc. Final Project):

📄 [Price of Abstention in Participatory Budgeting – PDF](Paper/Participatory_Budgeting_Final_Project.pdf)

## Tech Stack

Python · NumPy · pandas · matplotlib  
Simulation · Statistical Analysis · Computational Social Choice


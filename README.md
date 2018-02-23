# #LeanEstimates
## Or Lean Software Development Effort Estimation / Forecasting 
The purpose of this repository is to look at some interesting ways to estimate / forecast software effort. To be able to forecast we need a stable system and measure the flow of work items entering and leaving the system:
 
- A stable system is the foundation to our forecast. Try to keep arrival rate (work entering the system) and delivery rate (work leaving the system = throughput) the same.
- Limit work in progress (WIP) – Too high WIP and work is idle, to low WIP people are idle in your system.
- Measure throughput
- Measure cycle time. The time spent form starting work to actual value is delivery to the customer.

> __Note:__
The foundation of this approaches are that you have already gathered data and the size of work items do not vary to match.  To be fair this approach is handy when you have started with a project and collected already some data. Then it’s a great tool to check if you still on track. The main problem with this approach is the cold start problem. You must have the work items up front and for some approaches we assume that the size of the work items are independent and identically distributed (iid) random variables.


## My Definition o #LeanEstimates

> __TLDR;__ My Definition of #LeanEstimates - reduce pure estimation used in software projects (judgmental combination, analogy-based estimation, size-based estimation models, [more]( https://en.wikipedia.org/wiki/Software_development_effort_estimation)) to a minimum and use previous data (cycle times, etc.) to estimate / forecast remaining efforts. 


When we use a lean mindset we try to reduce waste. For example, waste are activities or things which are not directly adding value to the customer. Of course, we will not get rid of all the waste but we try to eliminate it to a bare minimum.  It's like the daily standup. A standup is technically waste, but useful for the team. But you would not say that we should do standups twice a day, because they are useful? So, it's a thin line between waste we need and waste we don't want. Be pragmatic, not dogmatic! 

I personally want to __reduce estimation to a minimum and use previous data (cycle times, etc.) to forecast__ were we stand and when we might be done.

## Examples
This repository is collection of approaches to do work estimation with data.
- Forecasting with a Monte Carlo Simulation [(Juyper Notebook)](notebooks/forecasting_with_monte_carlo.ipynb)

The examples are inspired from previous publications form _Klaus Leopold, Vasco Duarte and Daniel S. Vacanti_. For more details have look at the reference section.

## References

- Practical Kanban: From Team Focus to Creating Value, 2017, Klaus Leopold
- '#NoEstimates': How to Measure Project Progress Without Estimating, 2015, Vasco Duarte
- Actionable Agile Metrics for Predictability: An Introduction, 2015, Daniel S. Vacanti



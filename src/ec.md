# Extended Capabilities

## Variable Class and Sampling Methods

Variables:
- Conditional - Activated/Deactivated based on certain conditions
  -  -1 = active
  -  0 = inactive
  -  > Note: Variable sampling method attribute must be set to `None`
  -  Static - Simplest case of profile property that can be set statically
  -  Dynamic Conditional - Defined because the condition is dependent on a simulation variable i.e. a variable is only active only if 2 or more units are commited to a specific power station
  
- Escalator - Automatically change a datum over time according to user-defined rules
- Stochastic - Stochastic or expected profile data
  - There are 2 approaches for randomising datum:
    1. Directly define chronological samples that can be randomly selected - can be correlated, but not necessarily and,
    2. Define expected value and info on how errors are distributed, allowing simulation to generate samples.

### Sampling Methods
- None
  - Value = 0
  - Only band 1 is used w/o stochastic modification
- Auto
  - Value = 1
  - Random samples generated as described above.
  - \# of samples generated is Risk Sample Count
- User
  - Value = 2
  - Each input profile band forms 1 sample in order
  - i.e. band 1 = sample 1, band 2 = sample 2 etc.

## Stochastic Modelling for Wind/Fuel Prices

The Stochastic Object has an Outage Method Options:
- Normal
  - Value = 0
  - Standard Monte Carlo Method to draw random sequences of outages
- Convergent
  - Value = 1
  - Pre-filter patterns of outage to remove statistically unlikely outcomes.
  - Idea is to take a number of candidate patterns for each final pattern used in simulation and compute Chi-square statistic, to choose pattern that is closest to the expected outcome.
  
## PASA Simulation

PASA: Projected Assessment of System Adequacy

PASA is run after the LT PLan

- Schedule maintenance events for subsequent simulation phases MT Schedule and ST Schedule
- Model planned and maintenance outages of generation plants and transmission lines, and their severity
- Calculates optimal reserve that should be shared b/w region using transmission network, to find a reliability statistic for the system.

It answers questions like:
- What is the optimal reserve share?
- When to schedule next maintenance event?
- How to prepare for an outage?

### PASA Settings in PLEXOS

- Resolution: How often peak periods are calculated
- Transmission: Regional, Zonal, Nodal
- Stochastic Setting: Deterministic, Sequential MC, Parallel MC, Stochastic
- 
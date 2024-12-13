# Long Term Modelling

## Capacity Expansion and NPV
Capacity expansion considers the:
- cost of retirements
- cost of new builds
- fixed operating costs and,
- variable operating costs

to: 
- Maximise the NPV (Net Present Value) of the total costs of the system over a long-term planning horizon.

$$ NPV = \frac{R_t}{(1+i)^t}$$

where:
- $R_t =$ net cash flow
- $i =$ discount rate
- $t =$ time of cash flow

NPV is used to determine the profitability of a certain project.

Capacity Expansion allows us to find out:
- How much to invest?
- What technologies to build?
- How many units to build?
- Where to build?
- When to build?

Within the LT object there are 2 components:
- Capital Costs $C(x)$ and,
  - One off fees i.e. new generators, transmission expansion, generator retirements
- Production costs $P(x)$
  - Operational costs i.e. operating existing and new builds of transmission network, notional cost of unserved energy.

The goal is to minimise NPV by formulating it as a Mixed-Integer Problem:

$$C(x) + P(x) = \text{Total Cost}$$

To formulate this you usually have an objective function: in this case to minimise costs and constraints that the equation is subject to. i.e. 


![alt text](image.png)

## Application in PLEXOS

In PLEXOS, there is an LT PLan Object where you can consider:
- Step Size: in years, can also consider overlap
- Chronology: Partial, Fitted Sampled
- Discount Rate: %, End Effects Method (Perpetuity, None), Discount/Expansion Period (Month, Quarter, Year)
- Transmission: Regional, Zonal, Nodal
- Expansion Algorithm: Linear Programming, Mixed Integer Programming

## Generation Capacity Expansion

To define a Generation Expansion you need a generator with the following:

- [Max Capacity] in MW 
- [Max Units Built]
- [Build Cost] in $/kW

If LT Plan uses Discount Rate, define:
- [Economic Life] in years
- [WACC] - Weighted Average Cost of Capital in % 
- [FO&M] - Fixed Operating and Maintenance costs in $/kW/year
You also need Heat Rate, Fuel Price and VO&M charges.

### Retirement

![alt text](image-1.png)

These tables display points at which a generator is retired. Table 1 shows the effective date (aka Planned Retirement) of the generator and Table 2 shows the Economic Retirement which shows the retirement costs, heat rate and fixed O&M charges to justify the retirement.


##  Application in PLEXOS

- Planned addition of AC and DC lines is supported by OPF methods in PLEXOS using Line [Units]
- PLEXOS auto recomputes shift factors to cope with change (in topography)
- LT Plan supports all types of transmission constraints including security-constrained optimal power flow.
- Optimized transmission line expansion (using the [Max Units Built] property), retirement (using the [Max 
Units Retired] property) in LT Plan works in much the same way as generation expansion.

Explansion is done in continuous units of megawatts, this all you need is:
- [Expansion Cost] in $/MW
- [Max Expansion] in MW
- [WACC] in %

Expansion uses **Interface** which helps with both zonal/regional transmission and full-nodal AC expansion.
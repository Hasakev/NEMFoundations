# Module 5: Ancillary Services

This module aims to:

- explain the need for ancillary services
- explain the range of ancillary services
- explain the pricing and enablement of Frequency Control Ancillary Services (FCAS)
- explain the concept of co-optimisation between the energy market and ancillary service markets and co-optimisation between regulation and delayed FCAS markets
- explain the way ancillary service costs are recovered

## Ancillary Services

Ancillary Services are an "insurance policy" for power systems. Certain generators are paid to provide the capacity to alter their supply in case they are needed. This way, if an unexpected event occurs, those systems can draw on those "backup" services to maintain supply. AEMO purchases the required services from providers under **Ancillary Service Agreements** and **Market Ancillary Service Arrangements**.

NEM Ancillary Services can fall under 3 groups:

- **FCAS: Frequency Control Ancillary Services** - used by AEMO to maintain electrical system frequency at close to 50 Hz at all times to adhere to NEM frequency standards.
- **NSCAS: Network Support and Control Ancillary Services**
  - Used to maintain system security and reliability of supply of transmission network according to security and reliability standards.
  - Also used to maintain or increase power transfer capability of transmission network to maximise the present value of net economic benefit to all those who produce, consume or transport electricity in the market.
- **SRAS: System Restart Ancillary Services** - used when a major supply distruption or a whole or partial system blackout occurs and power system must be restarted.

> Fun fact: AEMO found that procuring NSCAS was not necessary in 2022-23

AEMO operate 8 markets for the delivery of FCAS, NSCAS and SRAS are non-market services sourced via agreements with service providers.

## FCAS - Frequency Control Ancillary Services

FCAS is like a car engine, if a car travels at a constant velocity experiences a change in load but no change to the power input to the engine, it will speed up (load decrease, i.e. downslope) or speed down (load increase, i.e. upslope), if load changes in a power system, the frequency will deviate.

![alt text](image-1.png)

To maintain frequency, FCAS is used to alter either generation or demand to maintain supply/demand balance.

This can be done using the following subset methods:

- Regulation Frequency Control: Correction of supply/demand balance in response to minor deviations in either load or generation - These are continually used to correct minor changes in balance, usually controlled by AEMO's 2 control centres.
- Contingency Frequency Control:
  - The correction of supply/demand balance following major contingency events such as loss of generating unit or large transmission elements.
  - Providers supply contingency control serves may also be used to assist with regulation frequency control. Contingency services are controlled locally and are triggered by the frequency deviation that follows a contingency.

## Frequency Control Services

Frequency Control Services are provided by generators on Automatic Generation Control (AGC). The AGC system allows AEMO to continually monitor system frequency and send control signals out to regulation service providers to maintain a system frequency within the operating bands of 49.85 to 50.15 Hz

FCAS has 8 requirements:

**Regulation**:

- Regulation raise
- Regulation lower

**Contingency**:

- **Fast raise** and **fast lower** - six second response to arrest the immediate frequency deviation.
- **Slow raise** and **slow lower** - sixty second response to keep the frequency within the single contingency band.
- **Delayed raise** and **delayed lower** - five minute response to return the frequency to the normal frequency operating band of 49.85 to 50.15 Hz.
- **Very fast raise** and **very fast lower** will be introduced in October 2023. These services will respond within one second to arrest the frequency deviation.

## NEM Dispatch Machine

An FCAS offer or bid submitted for a raise/lower service represents the amount of MWs that a participant can add to the system in order to raise/lower the frequency in the given timeframe.

During every market dispatch interval, AEMOs NEM Dispatch Engine (NEMDE) must ensure there is a sufficient amount of all eight FCAS services to meet the FCAS MW requirement

![alt text](image-2.png)

## NEMDE and co-optimisation

When determining the quantity of Regulation and/or Contingency FCAS, AEMO must calculate the required quantity that:

- can be sourced from any NEM region (global FCAS requirement).
- can only be sourced from nominated regions (local FCAS requirement).

Local FCAS providers are required in abnormal circumstances where only local market participants are practically able to provide FCAS. This most often occurs when a region becomes isolated — or 'islanded' — due to planned or forced transmission element outages.

When the services are required, NEMDE will enable FCAS offers in merit order of cost. The highest cost offer to be enabled will set the price for the FCAS service type.

## FCAS markets settlements

For each five-minute market dispatch interval, NEMDE determines a clearing price for each of the eight FCAS markets. This price is then used by settlements to determine payments to each FCAS provider.

All payments to FCAS providers are recovered from market participants according to the recovery rules. As contingency raise requirements are set to manage the loss of the largest generator on the system, all payments for the three contingency raise services are recovered from generators. On the other hand, as contingency lower requirements are set to manage the loss of the largest load/transmission element on the system, all payments for the three contingency lower services are recovered from customers.

The recovery of payment for regulation service is based on a "causer pays" factor methodology (Contingency is also a form of causer pays principle). Under this methodology the response of measured generators and loads to frequency deviations is monitored and used to determine a series of factors.

![alt text](image-3.png)

## NSCAS: Network Support and Control Ancillary Services

NSCAS are used to control the voltage at different points of the power network to within the standards, or keep power flow on networks within the physical limitation.

NSCAS is provided either by NSPs or by AEMO through non-market agreements. They are not part of the market.

There are 2 categories of NSCAS:

- **RSAS (Reliability and Security Ancillary Service)**: purpose is to maintain the power system within acceptable technical parameters or to increase access to supply such taht NEM can maintain power system security and reliability of supply in acordance to standards.
- **MBAS (Market Benefit Ancillary Service)**: purpose is to maximise present value of net economic benefit to all those who produce, consume or transport electricity in the electricity market. One way that MBAS can be delivered is by increasing power transfer limits in order to reduce the impact of constraint equations on NEM dispatch. AEMO uses contratint equations to model limits in the NEMDE to provide physical limits of transmission networks in a mathematical representation.

## SRAS (System Restart Ancillary Services)

SRAS enable the power system to be restarted following a complete or partial system blackout. There are a total of twelve system restart ancillary services and these align with designated electrical 'sub-networks'.

## NSCAS and SRAS payments

Both NSCAS and SRAS are provided to the market under long-term ancillary service contracts negotiated between AEMO and the participant providing the service. These services are paid for through a mix of:

- **Enabling payments**: made only when the service is specifically enabled
- **Availability payments**: for every trading interval that the service is available
- **Testing payments**: made when a test is successfully conducted
- **Usage payments**: made when the service is successfully delivered in response to an instruction from AEMO

NSCAS payments are recovered from market customers only, whereas SRAS payments are recovered equally from customers and generators.

#

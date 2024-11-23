# Module 5: NEM Spot Pricing and Dispatch

This module aims to:

- explain the NEM model which links and matches the supply and demand for energy
- explain how the NEM model maximises the value of trade and delivers an optimal market solution for users
- explain the dispatch and pricing process
- identify the relationship between bids, dispatch and the calculation of the spot price
- explain how network loss factors affect the spot price
- identify the roles and responsibilities of all parties in dispatch and pricing
- explain the Spot Market Timetable and market data publishing cycle

## Spot Pricing and Dispatch

All wholesale electricity is traded by market participants through a central pool comprising a number of pre-defined pricing regions.

The spot price, used to settle trading participants located in a particular region, is the dispatch price calculated for that region every five minutes. The dispatch price is set at the value where competitive offers to supply electricity match demand.

All electricity generated and consumed within a region is paid for at the regional spot price. Trading in the wholesale electricity market can be risky because the spot price can be volatile.

The electricity pool is made of a set of rules and procedures managed by AEMO in conjunction with generators, customers and NSPs. These rules act to centrally operate the power system and balance supply and demand.

Electricity is traded using a pool to enable competition. This is because electricity cannot be stored, and so supply must vary dynamically to match demands. 1 unit of electricity is indistinguishable from any other unit so you can't tell which generator produced what electricity.

Electricity supply and demand must be balanced and matched instantaneously to provide a safe supply at acceptable quality standards

![s14390311232024](https://a.okmd.dev/md/67415c6a6c2f7.png)

For AEMO systems to facilitate supply, generators must submit bids to AEMO specifying the volume of electricity their generating units are ready to produce for a specific price. A big covers a trading day (4AM to 4AM AEST). Generators can submit bids using 10 price bands.

- Bids submitted after 12:30pm AEST for the next trading day are called rebids and must be accompanied by a reason.
- All bids for the current and (after 12:30pm AEST) next trading day are also reflected in pre-dispatch schedules.
- Pre-dispatch is an indicative forecast of dispatch and pricing for the current trading day (and next trading day, after 12:30pm AEST) to a half-hourly resolution, and updated every 30 minutes.
- Pre-dispatch shows at a five minute resolution for the next hour.

![s14422211232024](https://a.okmd.dev/md/67415d310e93f.png)

AEMO manages the central dispatcch process and pricing cycle that runs every 5 minutes. The central process determines, b ased on a least-cost optimisation of all bids submitted for supply and demand. The production required for each unit to meet AEMO's forecast of demand at the end of each dispatch interval. This is called **scheduling**.

Bids are stacked in order of rising prices, that sufficient generation scheduled to meet the net demand. This means more expensive generators are only scheduled if and only demand increases.

At the same time, the central dispatch process optimally determines, based on bids from ancillary service providers, the capacity reserves required to handle the potential loss of a generating unit, load or transmission network element

The results of the optimisation are used to determine the dispatch price and ancillary service prices for each region.

## The Spot Market and Spot Price

- Spot Market: where the market generators are paid for the electricity they sell to the pool and customers pay for their electricity consumption from the pool. All electricity is traded at the spot price. Pool is divided into pre-defined regions.
- Spot Price: determined every 5 minutes, used to settle all actual energy traded in NEM
- Market Price Cap (MPC): maximum bid price set by the Rules, As of 2023-24, MPC is $16,600.
- Market Floor Price: minimum spot price, which is at -$1,000 per MW/hr.

## NEM Regions and Prices

As mentioned previously, each pricing region has a unique RRN, that has a regional reference price. All prices are accessible on the internet.

When calculating spot prices, AEMO needs to consider Interconnector capcity and also Loss factors.

- AEMO may need to schedule a more expensive generator to meet demand if the interconnector capcity limit is reached, even if there are cheaper options.
- Loss factors can occur during:
  - Inter-regional transmission (b/w regions)
  - Intra-regional (b/w generators and RRNs or RRN to customer)
  - Transportation within distribution network.

![alt text](image.png)

## Administered Pricing

Pricing is naturally volatile, and so factors like the Rules provide the spot market with a mechanism to cap financial exposure - this is known as **administered pricing.**

Prices in a region are limited by an administered price cap for the remainder of trading day if the sum of spot prices in that region over the previous week exceeds the Cumulative Price Threshold (CPT). CPT is adjusted for inflation every year.

There is also an administered floor price (the negative of the administered price cap) which floors pricing during the administered pricing period.

## Mandatory Restrictions (MRs)

The government can also employ Mandatory Restrictions (MRs) to reduce electricity demand in a region, where there are otherwise insufficient supply to meet demand.

This results in lower market prices that usual.
Mandatory restrictions process

The MR process is as follows:

- A jurisdiction enforces MRs on electricity use.
- AEMO and the jurisdiction agree on how much demand reduction is likely to occur (MR schedule)
- AEMO calls for MR bids from scheduled generators and network service providers within the region, and contracts sufficient MR capacity to meet the MR schedule based on the lowest cost bids
- AEMO rebids the contracted MR capacity into the central dispatch process at prices above the market price cap

## Projected Assessment of System Adequacy (PASA)

PASA is information supplied by generators and is data used to make decisions about when to maintain generating plants.

- **Pre-dispatch PASA (PDPASA)**: capcity adequacy forecast covering same period as pre-dispatch updated every 30 minutes, total regional generating capacity compared with forecast regional demand.
- **Short-term PASA (STPASA)**: 6 day adequacy forecast updated every 2 hours, to a half hourly resolution, total regional generating capacity compared with forecast regional demand.
- **Medium-term PASA (MTPASA)**: 2 year adequacy forecast updated weekly at a minimum, to a daily resolution, total regional generating capacity compared with forecast regional demand.

## Rights and obligations of NEM participants in pricing and dispatch

- Must participate in the central dispatch, pre-dispatch and PASA processes
- Must provide daily PASA availability and any weekly energy constraints for the next 36 months for use in MTPASA
- Must provide half-hourly PASA and market availability and any daily energy constraints for the next seven days, for use in STPASA
- Can apply to AEMO if they wish to aggregate their scheduled generating units for the purpose of central dispatch
- Must inform AEMO two days ahead of each trading day of available capacity for each trading interval of each trading day
- Must advise AEMO of any expectations that a generating unit will not be able to operate in accordance with dispatch instructions
- Must ensure their ability to dispatch electricity as required under the dispatch schedule
- Must have facilities that can receive dispatch instructions, both electronically and manually, every five minutes
- May submit rebids to change available capacity
- Must respond to dispatch instructions by following energy targets or providing enabled ancillary services if requested

### Semi-scheduled generators

These are the same as for scheduled generators, except:

- Must provide to AEMO an energy conversion model for each semi-scheduled generating unit as part of registration, for use in creating intermittent generation forecasts
- Must provide to AEMO the plant availability of each semi-scheduled generating unit over the next 36 months
- Are not required to separately provide PASA or market availability for use in PASA
- Must respond to dispatch instructions to cap the output of their semi-scheduled generating units to avoid violating power system security or economic dispatch — these instructions are flagged as 'semi-dispatch intervals'
- Cannot participate in reserve contracting

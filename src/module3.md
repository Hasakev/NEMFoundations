# Module 3: The Network

This module aims to:

- describe how the transportation of electricity takes place
- provide information on network ownership
- introduce network security concepts
- discuss network planning
- provide an explanation of network losses and their impact on the market
- explain how the network is regulated in the NEM
- discuss network revenue and pricing arrangements

## The Network

The Network: the infrastructure that transports electricity from generation sources to consumers. It comprises the poles and wires, as well as the apparatus, equipment, plant and buildings used to transport electricity to customers, excluding any connection assets.

The overall system has 2 main sections:

- **Transmission system** - high voltage, large power lines like the free-way
- **Distribution system** - lower voltage, power to suburbs, like small roads

A shared network allows the distribution of bulk generation in the most economically efficient and reliable way, allowing for energy supplied 99.9% of the time.

The network fulfils 3 roles:

1. Transport electricity from generator to customers.
2. Facilitate competition by separating generation and transportation.
3. Ensure a secure and reliable supply of electricity to consumers.

NEM were originally built as standalone systems, but eventually were connected up, hence electricity produced in a cheaper location can now be moved to a more expensive region.

Each region has a RNN: regional reference node, where the regional electricity spot price is set.

In general the RRN is a nominated major transmission substation located at, or close to, the largest load centre within the region. The regional price is calculated at this node and inter-regional energy transfers are also modelled between these regional reference nodes.

Transportation b/w NEM regions are called interconnectors, electricity is imported when:

- Local generators cannot meet that region's - demand, or
- The price of electricity in an adjoining region is low enough to displace local supply

Benefits of connecting the regional networks are:

- Increased supply reliability
- Inter-regional trade
- More efficient sharing of generation resources

**NSP: Network Service Providers** own, operate and control networks, there are 2 types:

- Transmission network service providers (TNSPs), who own transmission assets. There is only one of these in each NEM region
- Distribution network service providers (DNSPs), who own distribution assets. In some states there are several of these and in other states just one

## Economic regulation and pricing

AER: Australian Energy Regulator ensure pricing is regulated to prevent corruption.

They also regulate TNSP and DNSP licenses, meaning they may impose explicit requirements and service standards in addition to the Rules.

NSPs are entitled to recover efficient operating costs and earn risk-adjusted rate of return on capital required to provide services. AER usually checks NSP revenue every 5 years and sets a MAR: maximum allowable revenue (revenue cap) an NSP can collect from customers each year.

Imagine the power network as a public road that allows electricity to your home. Maintaining the 'road' uses certain costs, and these are factored into electricity bills. These charges are meant for different areas of the process:

- Consumers pay **Transmission Use of System (TUOS)** charges to the TNSP for the network usage at that point, charges recover the asset, operating and maintenance costs of the transmission network. (Typically 10% of total bill)
- Consumers pay **Distribution Use of System (DUOS)** charges to distribution NSPs (typically 40% of bill)

## Transmission loss factor

A portion of electricity is lost due to resistance and heating of conductors. Losses are approximately 10% of electricity transported. To allow for this loss, more electricity is generated than demand.

![s14114311232024](https://a.okmd.dev/md/674156019a6d8.png)

Losses occur when transporting electricity from a generator to the consumer due to the physical characteristics of the network. These losses need to be included when calculating electricity prices.

To incorporate the impact of network losses on dispatch and prices, losses are mathematically represented as 'loss factors'. There are several different types of loss factors in the NEM, calculated in different ways tor different purposes. These loss factors are grouped into two main categories:

- TLF: Transmission Loss Factor, all loss factors affecting transmission network are determined in April and applied each year on 1 July. A loss factor for a connection point is determined by calculating the increase in losses for an increase of 1 MW of load or generation at that connection point as supplied from RRN. This is referred to as Marginal Loss Factors (MLFs). Loss factors are used by AEMO to determine how much electricity retailers should pay at a certain connection point, and how much generators should be paid.

  > Generators also use TLFs to adjust bid prices to be competitive.

- DLF: Distribution Loss Factor, the average electrical energy loss b/w distribution network connection point and transmission network connection point. DLFs are calculated on the average loss b/w connection points over 12 months (unlike TLFs which are marginal). They are calculated annually by DNSPs before being communicated to AEMO.
  > AEMO uses DLFs to assist in settlement caluclations at each connection point.  
  > Retailers use DLFs to verify amount of energy being consumed at each connection point.

## Power System Security

AEMO's highest priority is security and reliability.

**Security** - the power system's capacity to continue operating within defined technically limits even if a single power system element is disconnected. (This event is known as a **credible contingency**)

**Reliability** - The power system's capacity to supply enough energy, even in peak times of demand.

Maintaining power system security means operating it in a way that does not overload or damage any part of it, or risk overload or damage after a contingency event.

Review of AEMO's responsibilities

A summary of AEMO's responsibilities in maintaining power system security is as follows:

- **Maintaining power system security** in a secure operating state and within the technical envelope
- **Maintaining reserves** by having in place a means of determining and maintaining sufficient reserve available to restore power system to a satisfactory operating state after a credible contingency
- **Load shedding** by having processes in place to arrest the impact of the loss of up to 60% of the - total power system generation.
- **Monitoring the power system** to assess that it is within the technical envelope, that scheduled generators and scheduled loads are dispatched in accordance with the National Electricity Rules, and that power system security is not jeopardised by operations on the interconnected transmission network and distribution networks
- **Reporting on and reviewing** events that pose a significant risk to the power system and major power system incidents
- **Procuring and utilising Ancillary Services** to maintain or restore the satisfactory operating state of the power system

## Network Planning

The process of investigation present and future network capability and identifying network upgrade requirements. Long-term planning is crucial to maintain security.

Network upgrades are driven by the need to:

- Maintain system reliability
- Increase market efficiency (by reducing network congestion and network losses, etc)

NSPs that upgrade need to adhere to the Rules. They need to address these requirements and information publicly via a economic cost-benefit test called RIT-T: Regulatory Investment Test for Transmission.

The Rules also require NSPs to conduct annual planning reviews that incorporate load forecasts, existing connection point adequacies, relevant transmission system adequacy, and planning proposals for future connection points.

AEMO is responsible for providing annual network development plans to guide investment in power systems.

AEMO provides The Integrated System Plan (ISP) is a whole-of-system plan that provides an integrated roadmap for the efficient development of the National Electricity Market (NEM) over the next 20 years and beyond.

They also provide a ESOO, that has a 10 year outlook period for projections of electricity usage and peak demands, generating capabilities of existing and committed generating units and an assessment of adequacy of electricity supply to meet demand (supply demand lookout).


## **Overview**

| NEMDE | EUPHEMIA                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|       | The European Commission has established a Target Model for a Single Day-Ahead Coupling (SDAC). This model has been laid down into the Framework Guidelines for Capacity Allocation and Congestion Management (CACM) in 2015. [2]                                                                                                                                                                                                 |
|       | Price coupling of regions is required to allocate scarce cross-border transmission capacity efficiently. The PCR EUPHEMIA (Pan-European Hybrid Electricity Market Integration Algorithm) is owned by NEMO members of the PCR and couples day-ahead wholesale electricity markets from different regions. The PCR operates by decentralised sharing of data into a single platform jointly operated by NEMOs.                     |
|       | Before the implementation of PCR-EUPHEMIA, interborder capacity has to be bid separately. Implementation prevents artificial market splitting and minimizes price differences across market areas, sending relevant price signals for cross-border transmission projects. The use of a Single Day-ahead Coupling mechanism also allows for overall trading efficiency and utilization of generation resources across Europe. [2] |
|       | There is also a Single Intraday Coupling for the execution of intraday auctions for the pricing of cross-border capacities.                                                                                                                                                                                                                                                                                                      |
|       | Continuously evolving with Euphemia LAB.                                                                                                                                                                                                                                                                                                                                                                                         |
|       | Further, there are constraints such as Long Term Allocation inclusion which ensures revenue adequacy for certain resources as part of its underwritten contracts. It also needs to corroborate between advanced bidding products, network models (ATC, Flow-based, Evolved Flow-based)                                                                                                                                           |
|       | NordPool and EPEX Spot are the main power exchanges that operates in the EU. The EUPHEMIA projects also includes EPEX SPOT, GME, HenEx, Nasdaq, Nord Pool, OMIE, OPCOM, OTE and TGE                                                                                                                                                                                                                                              |
|       | Also provides Single Intraday coupling to balance the wholesale electricity market.                                                                                                                                                                                                                                                                                                                                              |

## Considerations and content
### **How does bidding work in both structures?**

#### EUPHEMIA - Auction mechanism [3]

Deregulation of the EU energy sector looked to eliminate trade barriers between member states and build a common market
- Separation of production and supply of energy and the distribution and transmission networks. This discourages discrimination access and avoid cross subsidisation between transmission and power generation.

Markets assume perfect competition, sending the optimal allocation of resources and price signals for investment, which breaks down into
- every player has perfect information
- product is homogenous, divisible, and substitutable
- there are no significant market power (level playing field)

Electricity is an interesting commodity. Prices vary materially over time and location, and instantaneous matching of supply and demand is difficult.
- Demand varies and is not very sensitive to price signals (inelastic)
- Supply varies and is challenging to predict
- Difficult to store in large volumes
- Must be transported within the technical parameters of the grid. Physics based constraints. For example, voltage and frequency must be maintained. There are also thermal constraints
- There are also a diversity of different players, with different technologies, with different risk profiles and risk appetite.

There are four different types of markets
- Forward markets: Contract PPAs that performs long term risk hedging
- Day-ahead market: Companies can trade significant volumes on the day-ahead market if the forward market is not very liquid in that region. Or it can be used to refine positions in places where the forward market is liquid.
- Intraday market is used to adjust position based on new events to balance positions. More and more volume is moving into intraday market 
- Balancing market: Here, transmission operators take over and make sure that the system is maintained reliably. 
![[Screenshot 2026-08-27 094715.png]]

OTC - Over the counter, you have a direct relationship with the supplier, while in Exchanges, buyers are anonymised in the central process.
As you get closer to t=0, we get more constraints, it is related to a physics based system that satisfies the constraint of delivering enough power to the consumers.
- Continuous means that a buy order and a sell order match, and it takes place continuously, you can adjust to new information as they come
- While auctions is a used as a pay-as-clear system that pulls liquidity into a specific time. These are centralised processes. All accepted orders are paid as the clearing price.
- Day-ahead markets have implicitly transmission rights, while in OTC and forward markets, long term transmission rights are bought and sold separately.
- Forward markets operated by non-asset-backed operators will sell a contract a year in advance of a certain price, without means of generating that power. As t=0 gets closer, they will buy power on the day-ahead market to supply their consumers. This provides additionally liquidity onto the market

Contract for difference is s PPA, a financial instrument to incentivise investment for green energy, can be unilateral (government will top up when the strike price for producers is below the marginal price, a top up), while a bilateral contract, the producer will pay back to the government when the strike price is below the production price.

Europe has gone for the zonal approach, where each region has a single price per market time unit. This is due to legacy systems, reflecting national borders, whilst also supporting liquidity. A large bidding zone will allow greater liquidity from the market (debated). Bidding zones can evolve over time to reflect congestions.
- There are 30 TSOs that calculate capacity of their network and 16NEMOs that collect orders from market participants and use EUPHEMIA to calculate prices and flows between bidding zones.

Objective function to maximise social welfare.
- Competitive equilibrium: the acceptance of orders and market clearing prices are such that no market players would prefer other order acceptance levels, and supply is equal to the demand. To reach this competitive equilibrium, EUPHEMIA looks at the supply and demand curves
##### Auction mechanism

Incentive to bid truthfully the marginal cost of production as a high marginal cost mean that you won't get accepted.
![[Screenshot 2026-08-27 095909.png]]
Taking the intersection of these two curves. 
- Every order will be subjected to the same market clearing price.
- Fully accepted orders are orders making a profit.
	- Supply orders with a lower cost then the market clearing price
	- Demand orders with a higher utility than the market clearing price
- Fully rejected orders that would lose money, opposite to the fully accepted orders
- Partially accepted orders
	- They set the market clearing price so that they are economically indifferent to produce at any level
	
![[Screenshot 2026-08-27 100037.png]]
This is a pay as clear where every accepted order will pay/receive an amount equal to its accepted volume times the market clearing price
- Alternatively, pay-as-bid setting will pay/receive an amount equal to its accepted volume times the price of the individual order.

![[Screenshot 2026-08-27 100836.png]]

Definition of surplus for consumer and producer.

![[Screenshot 2026-08-27 101120.png]]

The welfare can be calculated from this surplus, where $$\text{Welfare} = \text{Consumer Surplus}+\text{Producer Surplus} + \text{(Congestion Rent)}$$
It is proven that finding the competitive equilibrium is the same as solving an optimisation problem for which the objective is to maximise the social welfare.

## Questions

- **How does EUPHEMIA and NEMDE recover costs of operation?**
- **What happens in islanding events?**
- **How does both engine deal with the co-optimisation problem, solving for both frequency management and the lowest cost?**
- **How does both optimisation engine respond to black-swan events, as well as issues of renewable integration? This is characteristic of resource availability in both markets as well**
	- **Drop out of coal fired generation**
	- **Duck-curve and midday lull in demand and over-capacity of solar**
	- **System blackout**
	- **Large transmission line failure**
	- **Drop out from data center connections?**
- **How does it handle regional variation in prices, demands, and supplies?**

## Sources

[1]N-SIDE. 2021. The Single Day-ahead Coupling (SDAC) and the PCR EUPHEMIA algorithm  https://www.n-side.com/en/insights/en-the-single-day-ahead-coupling-sdac-and-the-pcr-euphemia-algorithm/ 
[2] EPEX Spot. 2026. European Market Coupling. https://www.epexspot.com/en/marketcoupling
[3] N-Side. 2023. Power Market Auctions 101? [https://www.n-side.com/en/insights/how-do-power-market-auction-algorithms-work/](https://www.n-side.com/en/insights/power-market-auctions-explained/)
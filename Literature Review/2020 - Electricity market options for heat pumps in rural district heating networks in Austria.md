https://www.sciencedirect.com/science/article/pii/S0360544219325708

[[2024 - Review of Business Models for Industrial Heat Pumps]]
## Contributions

Discusses the participation of heat pumps in the day-ahead spot market and balancing market in several concrete use cases for district heating in Austria.
- Participating particularly int he automatic frequency restoration reserve

Also demonstrates sensitivities of heat pump profitability to several external factors and biomass pricing fluctuations.

The study designed business models, assigned use cases, and state of the art scenarios are developed based on assumptions of fuel prices, electricity prices, and call probability. An operational optimisation model is used to simulate these use cases. These concepts are
- DH network
- local heating network
- large customer
Which parameterises the number of customers, annual heat demand, supply and return temperatures, and capacity installed and type of producers.

Uses a mixed integer linear programming model. This model provides a cost optimal method for operation of the energy systems. The results are limited to the addition of a heat pump to a biomass boiler.

- Mostly found that biomass price and call probability are the highest influencing factors in the results. 
## Content

4.08 GW of installed wind and solar in 2018. District heating is also facing variable energy prices, lower efficiencies as the biomass plants are aging out, and decreasing demand (from decentralized energy production and CER?)
- Heat pumps allow the use of alternate energy sources such as sewage water, industrial waste heat, geothermal heat, and flue gases.
- They can also offer voltage management, congestion management, reduction of peaks, and provision of operating reserve. The Austrian market considers three products; the frequency containment reserve, the automatic frequency restoration reserve, and manual frequency restoration reserve

[28] shows that participation in the flexibility market cannot reduce costs due to minimum running time of the heat pumps.

Note that there are minimum pool size for FCRs. This will become a consideration for the aggregation of heat pumps in industry.

In the cases where the spot market price is low or negative, heat pump will always contribute to heat generation, which requires the operation of the biomass boiler as well.
- Again, the heat pump only allows for the improvement of efficiency (when used in the context of a biomass boiler)

Optimal strategy found was 50% of the energy in the day-ahead spot market and 50% on the negative energy balancing for the aFRR. 
- The same strategy whether or not the heat pump operation is coupled to the biomass boiler or not (flue gas vs sewage water)
- Decoupled operation of heat pump and biomass boiler enables more participation in the balancing market and take advantage of low electricity spot pricing (However, better business case for flue gas due to lower investment costs)

Note that adoption of heat pump in Austria may be limited by biomass subsidies in Austria, as well as established supply chains and high credit ratings with existing suppliers. Knowledge about the electricity market is also a big technical barrier to entry.
## Limitation

Assumes perfect knowledge of the electricity market and perfectly efficient plant operator behaviour. Therefore, represents the upper end of benefits.

Consider the use of an air-source heat pump with thermal storage and its participation in the frequency market.

We need to comment on if the efficiency improvements sourced from the heat pump would work from Iberdrola's perspective.

The paper suggests that high investment cost serves as an economic barrier to entry, and additional business models may invite more uptake.
## Questions

- Shows net positive NPV, taking this efficiency earning potential and fitting it into a heat as a service business model will be interesting

## Further Readings

Overall, there are a lot of literature on using heat pumps for demand flexibility in Europe, although concentrated primarily in the residential heating space and focused on consumer costs, rather than an overall market view.
- The difference between residential and industry heating is the heating demand requirements and temperature required, which makes the analysis different.

[25] look at the flexibility of residential heat pumps in a smart grid context in Germany
[26] Market analysis for short term flexibility options for residential heat pumps in Germany
[27] looks at a portfolio of residential heat pumps in Germany

[32] [33] pooling aggregators in Austria that includes heat pump in their portfolio.

There is also the IWPP-Flex project that concludes that residential heat pump pooling concepts provides a significant cost reduction. 

Need to look more into Multiple Integer Linear Programming

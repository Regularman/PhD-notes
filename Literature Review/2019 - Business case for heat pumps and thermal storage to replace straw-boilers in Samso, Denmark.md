https://www.sciencedirect.com/science/article/pii/S0960148119303027

[[2024 - Review of Business Models for Industrial Heat Pumps]]
## Contributions

Uses EnergyPLAN to investigate the introduction of heat pumps to fluctuating renewables and overall system cost.

EnergyPRO model is used to find the optimal business economic design and operation of the district heating plant, optimised against an external day ahead spot electricity market.

Given the locally fluctuating renewable energy sources (Wind power) and local biomass availability as a context, heat pumps have a positive impact. However, significant flexibility through heat pumps and overcapacity on heat pumps does not pay. The basis of the article is set on the Ballen Brundy District Heating System on Samso, the first fully renewable island in Denmark.
- The goal in Samso is to decarbonise heat and transport by 2030, 20 years ahead of Denmark and the EU. 
- Proposes to replace biogas burners reliant on local agriculture and energy crops in district heating facilities.

**Note the unique ecosystem that Samso is in; high electricity export, net-zero renewables, no industry demands and locally available biomass from agricultural sector.**
## Content

Europe district heating is looking at geothermal plants, waste heat from power plants or waste incinerators and industry, biomass boilers, solar thermal collectors, heat pumps, and electric heating. Literature also looks at Wind powered thermal energy systems (WTES).

Biomass are more appropriately used as peaking supply, a source of carbon for transport fuels, or in industrial process where alternatives are sparse.

In EnergyPLAN, looked at three different groups:
1) Replacing DH with heat pumps (however, due to asynchronous production from wind turbines, electricity imports are required). This will also reduce $NO_x$ and $SO_2$ emissions.
2) Adding thermal storage to existing DH systems (powered on biomass but that is needed to produce biogas and there is excess wind power in the region). The size of thermal storage required is analysed.

Heat storage is two orders of magnitude less expensive than electrical storage. [59]. Furthermore, the addition of thermal storage reduces the start stop of heat pumps and lengthen its lifetime. 

The electrification of the heating sector aligns with the wider climate goals in Denmark. In Samso, climate renders cooling unnecessary and industry is negligible.

Has good data on biogas boiler operation in Denmark, although situation may be unique due to locally available feedstocks (energy crops). As well as price data for thermal storage steel tanks.

![[Screenshot 2026-06-05 122832.png]]

Loaded in the heat demand profile and electricity spot market price variations.
- Just the heat pump being installed is able to displace electricity exports but adds to the total cost of operation (but this maybe because of local availability of biomass)
- When looking at the marginal cost of production, a heat pump has a lower marginal cost compared to a straw boiler only in the summer due to higher resource temperature and higher Lorentz efficiencies with high ambient temperatures, which leads to higher COP factors
- Highlights that heat pump alone is not sufficient for the meeting of demand, and therefore includes an electric boiler as well in one scenario.

Ultimately showed that it does not pay to invest in oversized storage beyond 24h. However, the study only looked at thermal storage interaction with the electricity spot market. There may be other mechanisms to provide financial incentives.
- However, the conclusion was not convincing. The argument that overcapacity of storage will not be financially feasible does not include discussion of selling electricity back to the grid. It shows that the costs levels out when increasing heat storage. The interaction of the heat storage with the electricity market is not explicitly highlighted, it would be interesting to look at interactions of thermal storage under negative price market signals and how the thermal storage solution can interact with that. 
- Furthermore, PPAs with the wind farms can be considered to analyse how that will affect the system pricing.
- The study also needs to look at the carbon abatement impacts and how that can affect revenue from carbon pricing.
- The heat pump operation also seems to be constrained by the heat demand, which is why oversizing the heat pump and storage will not have any revenue feasibility. What happens if capacity of the thermal storage is reserved to do arbitrage? Again, this would be interesting to look at in terms of an aggregate market perspective. 
## Limitations

- Does not provide extensive economic analysis and financial modelling of the heat pump project in analysis of heat pumps.
- Does not include efficiency of scale in the financial analysis
- Also does not explain the inner workings of why there is diminishing returns with larger thermal storage. The study requires more in-depth explanation on the ownership model and cost structures surrounding the heat pump.
- Would be interesting to perform sensitivities of analysis
- does not show market impact when these heat pumps are aggregated
- The study does not look at sourcing electricity from the nearby wind farm and when they are curtailed?
## Questions

- The sizing of the heat pump is insufficient to use the storage, but does not include how increasing the sizing will impact cost and feasibility
- How does power to heat work with a heat pump and  

## Further Readings

[11] [12] includes how heat pumps and heat storage can form the basis of a RES-based heating system in China and Europe.

[27] Electric vs heat storage in smart energy systems

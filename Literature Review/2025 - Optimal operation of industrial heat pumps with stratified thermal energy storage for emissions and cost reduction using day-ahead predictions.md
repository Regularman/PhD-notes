
## Contribution

Uses linear programming to develop operation schedule for heat pumps to explore the benefits of load shifting using TES
- objective function to reduce carbon emissions and to reduce operational costs

Looks specifically at industrial scale heat pumps.

There are many literature that already looks at the optimal operation of heat pumps with various renewable technologies.

- Addresses gaps in techno-economic analysis and analysis of stratified TES (hot ware stored in distinct temperature layers $90\degree$C to $62.7\degree$C). Stratefication occurs naturally due to convection and density difference

Setting is in a brewery. Also does not assume complete knowledge of inputs such as heat demand, renewable energy availability, and electricity prices. This allows more realistic simulation of optimal behavior. (It did a base case, perfect forecasting scenario, and realistic prediction horizon)

- Also introduces sensitivity analysis
- Heat pump system based on a brewery in Faxe, Denmark. It has a natural gas boiler that heats water to 145$\degree$C. It also has a 12MW PV park to reduce its electricity consumption.
	- It will install a 1.75MW ammonia heat pump 
## Content

Provides the formula for COP, although with an accuracy of $\pm10$% and is applicable to ammonia as a working fluid. It provides a higher level of detail than assuming a constant Lorenz efficiency

You also have to consider the ramp-up ramp down and minimum load of the technology.

- Empirical evidence for the 

## Questions

## Further Reading

What about the greater market impacts
[7] investigates investment costs
[8] focuses on grid flexibility and renewable energy penetration
[18] Potential for the flexible operation of heat pump to provide ancillary services
[22] HTHP, TES, and wind turbine to supply super heated steam
[20] Performance of an integrated heat pump and storage tank system for optimising heat recovery with multiple HTHPs in a dairy farm

[23] Example of brewery in Denmark
## Gaps

Does not look at dynamic load profile, assuming that the heating demand, electricity consumption and solar radiation to remain static within a 36 hour forecast horizon

- The heat pump base case operational strategy seems to be random
- Objective function is constrained to minimise the intraday energy level change in the tank after 36 hours

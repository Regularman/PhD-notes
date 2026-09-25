https://www.scopus.com/pages/publications/85056507049?origin=resultslist

## Contributions

MOO to minimise the TAC and total annual $CO_2$ emissions using a weighted sum method.
- This provides a trade-off method for planners between economic viability and environmental sustainability.
- Also compared with a baseline reference case

The demands is a cluster of $5$ residential buildings, a super market and a hotel in a neighbourhood in Turin. The simulation accounts for seasonal variations in energy demands.

The variables of designing a heat production network are 
- Identifying number and size
- Design of interconnection network
- Type of energy devices

The HPN have to satisfy multi-energy demands (electricity, DHW, SH, and Space Cooling) whilst considering cost and emission aspects.
- Uses pareto frontiers to introduce tradeoffs. Co-optimisation uses weighted sum method. The pareto frontier can be found by changing the weight between $0-1$.
![[Screenshot 2026-09-25 100339.png|401]]
,![[Screenshot 2026-09-25 102849.png|287]]

However, this assumes that every user has a DER system and neglects the possibility of a centralised case.
- The distance between DERs are known and the distance between DER and the users are unknown

The costs is based on
- $C_{pipe}$
- $C_{ED}$ (energy devices)
- $C_{OM}$
- $C_{En}$ (Annual energy cost) Natural gas consumed and taken from the grid

Cost is stepped out into quasi-steady state simulations that simulates price during different time of day and year

While the environmental objective is based on the 
- Emission due to the consumption of natural gas
- Carbon intensity of the grid

Note that the design size of the technology must be within the minimum and maximum sizes available for the market,
- Also includes area constraint for solar thermal and PV panels.
- Includes the thermal losses in the piping network
- However, the heating network only allows for heat delivery in one direction
## Results

Shows that the topology of the network changes the tradeoff between cost and carbon emissions.![[Screenshot 2026-09-25 103323.png]]
![[Screenshot 2026-09-25 103333.png]]

However, in all cases, CHP is moved by the ICE rather than the CHP due to the lower capex and higher total energy efficiency of the technology. This contradicts other papers as the it does not consider waste heat recovery.

- The space available also makes a big difference, as this determines where the solar panels can be placed.
- It is more economically advantage to store heat produced from CHP plants rather than install large heat pumps, but this means that the size of the absorption chiller must be larger.
- There are also electrical efficiencies inherent in installing 1 large CHP plant compared to 3 smaller CHP plants.

The installation of pipes allow for avoiding the installation of boilers, as the DER enables systems to cover each other's peak demand loads.
- Sharing also allows for the decoupling of thermal-electric systems, as it is possible to civer large shares of the electricity and send surplus to other users.
- But there is a tradeoff with lower cost and higher emission due to the CHP unit operation.

Ultimately, the interconnected DER system performs better than baseline systems of grid power for electricity demand, gas fired boilers for DHW and SH demands and electric chillers for SC demands.
- 31.8% reduction in annual cost and 33.2% reduction in $CO_2$ emissions.
![[Screenshot 2026-09-25 104804.png|447]]
#### Operation strategy

Note that the study also optimises the operation strategy of the DER system, however, it is unclear how the control algorithm works and if a-prior knowledge of the demand is known (what is the charging strategy of the battery)
## Limitation

Does not look at the embodied emissions of each technology.
## Further Readings

[6] Looks at optimal configuration and operation of DER. But neglects the interaction between devices and end users through the heating pipeline. Minimises cost and pollution

[7] Looks at a single DER system in the absence of the pipeline network and minimises cost and exergy input.
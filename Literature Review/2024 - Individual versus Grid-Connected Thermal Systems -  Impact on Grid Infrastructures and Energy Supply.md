https://ieeexplore.ieee.org/document/10668974/
## Contributions

Used an in-house power flow analysis software to compare the peak demand of centralised versus decentralised heat pump. Showed that although electricity consumption decreased in the network case due to balancing of waste heat and cooling demands in the grid, the overall increase in loading on the power network increases due to the demand being concentrated in one place.
- Found that switching to a low temperature anergy network reduced the total electricity consumption
- Also found that the use of TES is effective at reduction of peak demand due to load shifting in the centralised scenario
The in-house power simulation software loads in waste heat potential, cooling and heating demands, then takes that and uses the Newton-Ralphson algorithm to calculate the power flow through the network.

The study is quasi-dynamic as the COP depends on external temperature. There are three main scenarios
- 

Case study is done on campus Forschungszentrum JÅNulich![[Screenshot 2026-09-29 at 8.44.19 am.png|423]]
## Content

The original heating network is operated between 95 $\degree C$ and 132 $\degree C$, while the temperature of the LTDHC network is decreased to 20 $\degree C$ and 30 $\degree C$. As the waste heat temperature of the HPC varies between 30 $\degree C$ and 40 $\degree C$, a simple heat exchanger with an efficiency of 80% is sufficient to integrate the waste heat.

The thermal network consists of 421 nodes and 451 pipelines, summing up to a total pipeline length of 33.7 km. We keep the parameters of the pipelines according to the real heating network, but increase the diameters of the pipelines nearby the HPC to 0.1m (this is relevant for a pipeline length of 1.7 km).

![[Screenshot 2026-09-29 at 8.42.53 am.png|399]]![[Screenshot 2026-09-29 at 8.43.09 am.png|406]]![[Screenshot 2026-09-29 at 8.43.27 am.png|399]]

Furthermore, it should be noted that the pipe diameter was increased in order to reduce pressure loss, hinting at the possible need for retrofits of piping networks in brownfield developments to improve efficiency.
## Limitations

The charging strategies of the TES is rule based. More interesting MPC control options can be used to explore full value proposition of TES.
## Further Readings

Assessing the grid impact of electric vehicles, heat pumps & PV generation in dutch LV distribution grids,

Quantifying the impact of residential space heating electrification on the texas electric grid

Decarbonizing heat with pv-coupled heat pumps supported by electricity and heat storage: Impacts and trade-offs for prosumer and the grid
https://ietresearch.onlinelibrary.wiley.com/doi/epdf/10.1049/iet-gtd.2014.0607
## Contribution

Design of an interconnected energy hub utilising technical and economic variables whilst respecting reliability constraints.
- However, in this case, energy hub is  a single building (such as a hospital in a city), which has electricity, heat, and cooling demand, and which can be met through a combination of technologies. These includes
	- CHP
	- boilers
	- compression chillers
	- Absorption chillers
	- Heat storage
	- transformer
	- heat exchange
	- Li-ion batteries

![[Screenshot 2026-10-07 131932.png]]
The goal is to maximise the NPV by deciding whether or not to include each piece of equipment in the energy hub.
- One of the KPIs used to the define the evaluated system is the Expected Energy Not Supplied (EENS) index. The penalty for lost loads is assumed to be 30 times the price of energy carriers

The study uses a simplified model of three energy Hubs representing a municipal district![[Screenshot 2026-10-07 132020.png]]

Assume that the cost of lost loads is 30 times that of the energy carrier (In this way, lost of load can be optimised for in the cost.)
- However, this has the limitation as we cannot tell what variables or network characteristics influences network reliability.

Further, there are two scenarios, with and without district heating in the energy hub ecosystem.
- And then they did load uncertainty and price uncertainty sensitivity through Monte Carlo analysis

Although resilience to load uncertainty is a measure of network reliability, it does not relate network design to improving network reliability through the EENS measure.
## Content

Monte Carlo simulation in load uncertainty shows minimal change in optimal system capacity in the case with a boiler (NPV is reduced by 3.64% which does show that load uncertainty reduces the profitability of the network). Therefore, what are the strategies to mitigate this risk?
- While in the case without district heating, the size of the absorption chiller will have to increase by 6.18-7.3%, while the size of the boilers will have to increase by 3.89 to 7.32% to account for the uncertainties. NPV will reduce by 4.57%.
## Limitations 

Although reliability is defined with EENS above, it is never actually applied in the results discussion and analysis.
- However, the system does the vary the load uncertainty to show that the CHP and boiler system can be used to respond to varying demand without extensive financial implications.

Further, the paper does not highlight the role of batteries in the system, only the installed capacity of the CHP and boiler under each scenario.

Further, report highlights that TES should not be installed when there is district heating, which misses out on opportunities of load shifting, an effect no considered in their modelling.
## Further Readings

[12] Reliability of energy hubs
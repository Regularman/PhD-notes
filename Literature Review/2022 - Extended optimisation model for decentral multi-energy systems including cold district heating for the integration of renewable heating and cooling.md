https://ieeexplore-ieee-org.wwwproxy1.library.unsw.edu.au/stamp/stamp.jsp?tp=&arnumber=9960562

Cited by 1
## Contribution

Looks at a multi-criteria optimisation procedure to minimise costs and $CO_2$ equivalent emissions

Applied algorithm on a case study with 20 single and multi-family houses
- You also need to consider that for direct cooling and heating to be possible, you need underfloor heat exchangers.
- This is almost a comfort as a service setup
## Content

The MCO model includes the inputs
- Geo-referenced data of buildings (location, size, insulation reinforcement status, and currently installed technologies, as well as yearly consumptions and load times)
	- Electricity, heating, warm water, and cooling demands are integrated as a quarterly time series of a reference year
- Technologies are fully described by economic and ecological parameters. The price and annual price dynamics are set
	- Current subsidies and levies are also integrated
	- The technology choice includes gas condensing boilers, air heat pumps, ground source heat pumps, pellet heating, wood-chip combustion, solar thermal, PV, and more.
### Method

1. The routing decision is based on a genetic algorithm
2. Technology expansion (Masterproblem of a Benders decomposition approach for a MILP)
3. Operation is optimised (Bender's subproblem) $\rightarrow$ further decomposed by Lagrange relaxation in the case of a cross building operation

- Did a sensitivity analysis on whether to include insulation or not.

Note that cooling can be achieved through heat exchanger platers, although this means that the temperature of the thermal fluid must be lower than the cooling demand.

Heat loss can be calculated using DIN EN 13941-1 and depends on the ambient ground temperature.
### Results

However, in the results, the paper DOES NOT show how they optimised the technology mix and setup used to provide district heating

- Also does not include grid temperature as an input variable, so they had to search for multiple grid temperatures
	- Showed time shifting of PV and heat pumps during low price period
	- Does not justidy cost and determine payback period
- ~={orange} It would also be interesting to look at what happens under various weather conditions. In this study, they used weather traces, but what would happen in different ambient temperature for more variability, for example=~
## Questions

1. What about the availability of heating demand given the technology type
2. How to determine the pumping power, since that is another consideration
3. Equation 4 and 5 does not make sense, a it is saying that, $$\dot{Q_{out}}=P_{el,chiller}(1+\text{Energy Efficiency Ratio})$$or notably they are correlating electrical power to thermal power with $$\dot{Q_{cooling}}=\dot{Q_{out}}-P_{el,chiller}$$
## Limitations

Grid temperature is assumed to be constant

Does not consider the location of the district heating plant 
## Further Readings

[5] [6] [7] Real world integration of district heating networks
[8] [9] [10] Energy savings, economic advantage, and renewable energy integration in a multi-energy system approach.
[11] describes the multi-criteria optimisation framework used in this study
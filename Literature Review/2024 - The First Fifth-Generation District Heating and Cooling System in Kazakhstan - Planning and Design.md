https://www.scopus.com/pages/publications/85141850165?origin=resultslist

## Contributions

Uses GIS to promote efficient and sustainable energy management in Kazakhstan, particularly through
- Decision making in the context of energy market regulation
- Operational data utilisation
- Modelling/simulation for technical design

Applies GIS decision making tool in designing 5GDHC in Northern Industrial Zone of Karaganda, Kazakhstan.
- This is integral for identifying the optimal locations for heat pumps, storage systems, and distribution networks.

The proposed model incorporates waste heat recovery from local sources, including nearby wastewater treatment plants, showcasing a sustainable energy solution for the industrial park in simulation
![[Screenshot 2026-09-23 114001.png]]

Focused on heat pumps in ultra low temperature district heating networks.
- Energy is stored in a aquifier pond

The paper highlights the operational strategy (set back temperature) of the 5GDHC and how it impacts the metrics outlined in the content section of this notes summary.
## Content

There are different types of models for heating networks
- Steady state systems are good for representing constant conditions but cannot represent transient behaviour and thermal inertia.
- Quasi-dynamics is a compromise between SS and dynamic systems
- Dynamic systems can account for transient changes in load, heat losses, and pump efficiencies. But they are computationally very expensive to run.

Models can be validated with 
- experimental data
- compared with other models known to be accurate
- sensitivity analysis

The study includes a heat pump set-back strategy when the building (commercial or residential is not used), considering
- Climate
- Insulation of the building
- Personal comfort level

Looks at the following metrics,
- Maximal heating and cooling demand 
- Volume heating and cooling demand
- Net volume heat on the grid 
- Maximum electric demand 
- CO2 emissions from heat pumps and circulation pumps
- Costs related to heat pumps, pumps, and valves

Fixes network temperature, electricity prices, and constant supply temperatures.

## Results

Results show that using the 5GDHC compared to the reference case offers savings and reduces CO2 emissions, with a payback period of 15 years.

- The simulation in GIS is quasi-dynamic, as the tool is able to figure out the flow direction of the heating network between base and peak flow rates.

Did not specify how to minimise hydaulic loss. Rather than answering what is the most sustainable way to meet the heat of this industrial district, it applied 5GDHC to show emissions and cost savings.

Outlines pipe radius to be a factor for the capacity of flow rate but does not explicitly outline how to best optimise this pipe radius.
## Limitations

Only looks at the space heating demand. (Also only looks at the peak demand rather than the load profiles of each plant)

The study is also technology agnostic, the specifications of the heat pump is not specified.

The study is not a comparative study that breaks down what is meant by the design of a good heating network.
- The placement of the booster heat pump is also specified to be distributed. There is also a centralised heat pump. There is no comparison on what is a good district heating network

Therefore, it can be said that this paper is limited to the techno-economic analysis of application of 5GDHC in an industrial park in Kazakhstan.

- What is the over-capacity and utilisation of the technology? Since the study is on space heating, there is only one quality of heat required, which is not what industry needs.

Does not five into the logistics of heat pump installation




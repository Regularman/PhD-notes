
https://www.aivc.org/sites/default/files/p_2433_0.pdf

## Contribution

Provides a linear programming model to emulate a DHN to support the design and decision making.
- However it should be said that the efficiency of the heat source is a non-linear system, and linearisation simplifies the problem and approximates the optimal
- Note that the objective of this paper is not optimisation, but evaluation of a system

- However, immediately frames DH as the solution to decarbonisation, due to its ability to integrate biomass, waste heat, or geothermal energy
The LP is applied to a French District heating network that is 22km long and has 116 substation, providing 130,000 MWh of heat

Analyses three scenarios based on
- Main heat production is the waste incineration plant and extra heat is supplied by a thermal plant using a fossil fuel boiler
- Storage is added to scenario 1, with capacity of 400MWh
- Waste incineration plant reduced 50% capacity and extra heat is supplied by a thermal plant and thermal solar panels.
Simulations are carried out over the year in hour timesteps.

## Content

In the model, the DH system is represented as an orientated graph and its energy behaviour is simulated at each timestep using LP.
- There are $n$ nodes (substations) and $m$ branches (pipes)

The unknowns to be solved are
- The heat flow in each branch
- Power production from each heat source

The system minimises heat production cost at each timestep, with respect to the constraints of maximal heat production capacities, fuel costs, conservation of energy.

The analyse have loads that vary, such as
- An incineration plant that uses municipal solid waste from local hospitals and other industrial wastes
- Two hospitals with their own 6MW and 10MW boilers
- Also consider that 69% of the network operates at high temperatures and pressures while the other 31% operates at lower conditions

The heat demands are space heating, water heating, and process heating. 
- However does not include investment and fixed cost of the system

### Results

Found that in Scenario 3, solar thermal panels have limited contributions due to the low temperature output of the panels and the high temperature of the network

![[Screenshot 2026-09-24 095810.png]]

Also shows the cost of each scenario, demonstrating the operational cost of each system.

![[Screenshot 2026-09-24 095834.png]]
## Further Readings

Outlines that decision support tools available for the design of DHNs, including
- Network topology optimisation [Soderman](https://www.sciencedirect.com/science/article/pii/S0301421513003418)
- Optimisation of pipe 
	- through the PipeLab model 2010 through energy loss 
	- Cost and economic variables, namely the total cost of the system through Persson's model in 2011
- Network design optimisation [Gustafsson](https://www.sciencedirect.com/science/article/pii/0360544292900658)
- Energy mix optimisation
- Mid-term operational planning tools [Dotsauer](https://www.sciencedirect.com/science/article/pii/S0360544203001518)




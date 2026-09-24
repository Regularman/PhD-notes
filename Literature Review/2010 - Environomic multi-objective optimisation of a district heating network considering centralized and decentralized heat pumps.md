
https://www.sciencedirect.com/science/article/pii/S0360544209004216

## Contribution

Uses a multi-objective and multi-modal evolutionary algorithm to facilitate the design and planning of a district heating network mased on a combination of decentralised and centralised heat pump, combined with onsite cogeneration.
- The algorithm is called a clustering Pareto Evolutionary algorithm (CPEA)

Uses cost and pollution metrics.
- Also considers life cycle from manufacture to operation and removal

![[Screenshot 2026-09-25 083630.png]]

- Uses Swiss electricity mix 

The overall demand on the grid is 62.7MW and the electricity cost, fuel costs, and pollution costs are fixed (NOX and CO2 emissions).

Users have different requirements, and the paper explores the distribution of user requirements with the performance of the heat production networks.
![[Screenshot 2026-09-25 085024.png|368]]
## Results

Sensitivity and optimisation analysis shows that network supply temperature was clearly the dominant independent variable. Some other variables that were considered was
- Share of heat pumps, gas turbines, gas engines, and boilers in the network, considering their manufacturing and disassembly costs.

Showed that the optimal solution without pollution costs occurred at $89.5\degree C$. This is as the cost includes buildings, equipments, networks, administration, and energy costs. However, the paper does not specify how these costs are calculated.
- High supply temperature meant that hot water demands can be met with heat exchangers on the supply line without heat pump use. The mass flow rate of user 3 and 4 is enough to allow the second user to make use of the return line heat exchanger. 
- However does not consider heat loss and efficiency?
## Limitations

Simplification to the superstructure is made, such as
- Removed return line heat pumps on the user side
- Network is in series and driven by an electric pump
- Electricity could be used internally, or to supply users of the heating network, but not be sold back to the electricity grid.
- Qausi-steady state as demand is modelled as simplified adjustements to the nominal operating regime. Accounts fr temperature variations in the COP but does not look at effects such as early morning overheating.
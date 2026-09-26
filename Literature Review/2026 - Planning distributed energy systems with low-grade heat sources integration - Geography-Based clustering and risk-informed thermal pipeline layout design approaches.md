https://www.sciencedirect.com/science/article/abs/pii/S0360544226001064?fr=RR-2&ref=pdf_download&rr=a40cc0c87e1e866f
## Contribution

MOO of for the following two task
- Clustering and partitions of source and load. The metrics used to inform this are
	- Ratio of Temperature to Delivery Distance
	- Source Load Matching Ratio
	- Average Euclidean Distance
- Within each cluster, the layout of pipes to minimise transmission length and risk of interrupted thermal load. The metric used to inform this decision problem is 
	- Sum of the investment cost and cost of interrupted heat load based on probabilistic modelling
	- Further, the placement of energy hubs in each cluster is chosen based on investment costs of pipes and their required diameter (required diameter specified by heat load and associated pressure loss)
	- The transmission network can be constructed as a Straight Line Minimum Spanning Tree (SMST), which has a lower investment cost, or a Road based Minimum Spanning Tree (RMST) implemented with QGIS.
		- Note that RMST may cost more, but have advantage of ease of land use as well as easier access for repair and maintenance.
## Content

The cost of interrupted load is prioritised based on asset type,
- Public building $0.34MMUSD/MWh$
- Commercial building $0.31MMUSD/MWh$
- Residential buildings $0.25MMUSD/MWh$

While the probability of heating supply interruption at any node is $$P_j=1-\Pi^{n_j}_{n=1}(1-pL_n)$$
Where $L_n$ is the line length, and $p$ is the heating supply interruption probability, and $n_j$ are the number of pipes from the node to the energy hub. 

Note that the weight between the operational objective and the planning objective (length of the transmission network) is balanced using a maximum fuzzy membership method.

Furthermore, showed that the operation metrics vary within acceptable tolerance under stochastic waste heat production. This demonstrates that this can be reasonably handled with electric heat pumps or CHP plants are the energy hub substations.
![[Screenshot 2026-09-26 at 8.00.24 am.png]]

Ultimately, the study demonstrated the lowest cost of the piping network, but does not take into account the technology used or the retrofit complexity for each load/ source. Some further considerations may also be 
- Exploration of energy storage potentials of heating networks
- Exploration of uncertainties in source load dynamics, such as season production variability
- Interconnection between district heating network and how that will impact resilience
## Limitations

- Does not provide information on the technology used for the district heating network, only that it is a bi-directional low temperature network suitable for waste heat recovery
- Furthermore, the study operated within a localised region, which is that the solution must be distributed 5GDHC. The impacts of the centralised heat production hub on the meeting the requirements of the users are unspecified.
## Further Reading

There is a critical gap for regional scale DES planning with multiple heterogenous heat sources.

[9] Transmission thresholds of heating networks
[10] Transmission distance and temperature parameters for industrial flue gas heat recoveries.
[11] Technology orientated view of industrial low grade heat
[25] Multi-level optimisation of DHNs
[19] Multi-period topology optimisation
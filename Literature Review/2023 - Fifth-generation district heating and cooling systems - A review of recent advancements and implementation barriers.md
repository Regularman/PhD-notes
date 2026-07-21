https://www.sciencedirect.com/science/article/pii/S1364032122008784
Cited by 192

## What is $5^{th}$ Generation District Heating and Cooling

$5^{th}$ Generation District Heating and Cooling systems operates at near ambient temperatures for lower heat losses in the network, and allows the integration of anergy into the district heating system, allowing for the participation of prosumers in the network. Through a bi-directional heat network, they can harness the demand synergies of different industries and residential areas. End users are equipped with de-centralised heat pumps connected to the low temperature bi-directional grid.

However, not much is known about their life cycle assessment and life cycle cost impacts.

Other keywords for 5GDH is 
- Ultra low temperature district heating
- Bidirectional district energy systems
- bidirectional low temperature networks
- Anergy grid
- 
~={orange}Ultimately, there is no holistic study with a detailed and transient model that considers mass flow, network pressure drops, and temperature distributions whilst also accounting for a full LCC and LCA of 5GDHC. =~

### Need for 5GDHC

There is an increase in space cooling demands due to increase in affluence and GDP. Traditional district heating systems operate in areas with high heat densities, and are reliant on fossil fuel. Therefore, reducing demand lowers the average heat demand density and threatens the business models of district heating.

There 5GDH should be able to work in a milder climate with lower heat demand densities.

| Generation | Heat transfer fluid                                                                                                                                                                                                                                                                                                                                                                                                   |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| First      | High temperature steam that has high temperature losses and safety issues.                                                                                                                                                                                                                                                                                                                                            |
| Second     | Highly pressurised water at 100 degrees. Used centralised condenser and decentralised evaporators.                                                                                                                                                                                                                                                                                                                    |
| Third      | Highly pressurised water at 80 degrees. Lowering of temperature to reduce heat loss.                                                                                                                                                                                                                                                                                                                                  |
| Fourth     | Looked at heating new buildings with lower heating demands and lowering the temperature of the thermal fluid to below 70 degrees, even as low as 50 degrees. This allowed some level of renewable integration and anergy integration.                                                                                                                                                                                 |
| Fifth      | Low temperature creates greater opportunities for recovery of low grade excess urban heat, solar thermal, and shallow geothermal energy. However, there is the drawback of higher substation complexity, thermal storage requirements, large pipe diameters, and higher pumping costs as a result of that. Lower temperature can also reduce insulation thickness and the environmental impacts associated with that. |
In 5GDH, it is important for energy storage such as Tank Thermal Storage, Pit Thermal Energy Storage, Aquifier Thermal Energy Storage, and Borehole Thermal Energy Storage to provide long term energy storage to balance out seasonal demands?

### New design and locational criteria

Traditional, DH locations are determined by metrics such as spatial heat density, specific heat density, or linear demand density (heat demand per unit length of network.) For example, you need new metrics for 5GDHC such as 
- Demand overlap coefficient to identify areas with complementary heating and cooling demands.

~={red}However, literature has still yet to identify what the best conditions for 5GDH is =~

### Approaches to modelling

| Model     | Type                                                         | Pros                                                                             | Cons                                                                                                                                                                                                  | Examples                                                       |
| --------- | ------------------------------------------------------------ | -------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| EnergyPro | Simulation                                                   | Incorporates economic evaluations into technical model of complex energy systems | Performs operation optimisation using an analytical method for unit commitment, where production units are dispatched according to a priority scale. Temperature effects are onlu modelled statically | [51]                                                           |
| IDA-ICE   | Simulation of building air quality and energy performance    |                                                                                  | Requires development of ad-hoc components in Neutral Model Format                                                                                                                                     | [52]                                                           |
| TRNSYS    | Simulation of substations, TES, and overall system behaviour | It is open source                                                                | Requires detailed data and training                                                                                                                                                                   | Used in Flexynet[19] and [53] ANN-MPC of 5GDHC demand response |
| Modelica  | Modelling language for complex systes                        | Can co-simulate behavior of buildings and district energy systems                | Requires detailed data and training                                                                                                                                                                   | [56], [57], and [58]                                           |
Optimisation functions can be LP, MILP, or other metaheuristic algorithms such as GA, Differential evolution, evolutionary algorithms, and PSO, which does not find the global optimal. These optimisation of the network is required for control and ensuring demands are met across the grid.
- Control methods are split into centralised and decentralised approaches. Rather than standard rule based controllers, more advanced optimisation techniques are required


| Optimisation Technique      | Pros                                                                     | Cons                                                        |
| --------------------------- | ------------------------------------------------------------------------ | ----------------------------------------------------------- |
| Linear Programming          | Physics based                                                            | Long computation time and some model simplification needed. |
| MILP                        | Physics based                                                            | Long computation time and some model simplification needed. |
| Whitebox-MPC                | Online optimisation system and physics based                             | Potential runtime issue                                     |
| Blackbox-MPC                | Online optimization system that is data driven                           |                                                             |
| Agent based control systems | Agents are considered to be cooperative or competitive with each other.  |                                                             |
There is also a hybrid approach where it is a 5GDHC spot market, with case studies in germany (Cologne) and San Francisco, using a Modelica simulation to show improvements in CO2 emissions and operational costs. 

### Environmental impacts of 5GDHC

[84], [85], and [86] Looks at lifecycle CO2 emiussions of renewable integration into district heating. However, the review highlights a lack of literature that focusses on environmental performance. Focus is on the operational performance of the system, and operational GHG emissions. As the grid decarbonises, it is important to look at the entire life cycle's embodied emissions in GHG and other planetary boundaries.
## Questions/Thoughts

A good literature review needs to outline the methodology of the review
## Recommended readings

### Proposals
[27] Reservoir network, new topology for district heating
[37] District energy network
[38] Multi-energy systems

### Case studies
[13] Existing case studies of 5DGHC in Europe
[19] Flexynet projects looked at 5GDHC
[74] Prosumers in DH, a swedish case study showing better energy and CO2 performance, although cost is higher.
[13] and [48] Minewater project in Heerlen, Netherlands. Uses a flooded decommissioned mine as a geothermal source for district heating and cooling. It used a three pipe backbone with a hot and cold supply and a common return line. In the new iteration, decentralised generation such as data centres, industrial projects, and supermarket refrigeration systems participate in bidirectional energy trade
### Possible LCA
[26] Exergy efficiency compared to individual heat pumps of 5GDH
[84], [85], and [86] Looks at lifecycle CO2 emiussions of renewable integration into district heating. However, the review highlights a lack of literature that focusses on environmental performance. Focus is on the operational performance of the system, and operational GHG emissions. As the grid decarbonises, it is important to look at the entire life cycle's embodied emissions in GHG and other planetary boundaries.

### Other interesting papers
[39] District heating system for ancillary services
### Controls and simulations

Look at the first three also for LCA of 5GDHC!

[51] Techno-economic modelling of a 5GDH system in central london
[20] MILP application to minimise TAC of 5DGHC [25] Quantifying demand balancing in bidirectional networks using Python [61] Temperature control optimisation in 5GDHC networks using MILP.
[54] Smart control of a district heating network with a high share of low temperature waste heat. White box MPC controls
[56] A novel method for designing 5GDHC
[23] Agent based control of bidirectional heat networks
[52] Looks at key performance indicators and complemntary load profiles for 5GDHC. Outlining the need to implement thermal storage and use ToU tariffs.



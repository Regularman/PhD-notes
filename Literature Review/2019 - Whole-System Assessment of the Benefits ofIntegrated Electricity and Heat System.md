https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8474307

## Contribution

Highlights how the integrated planning of heating and electricity power system reduces system OPEX due to lower VRE curtailment.

The study solves for the lowest system cost whilst applying 
- electricity and heat balances, 
- heating technology mix constraints (demand must be met by district network or end user),
- power flow constraints, 
- demand response constraints, 
- TES operating constraints,
- pre-heating constraints (thermal inertia of pipes and well insulated buildings), 
- generation unit constraint (ramp up and down time, ancillary serves and capacity in reserve)
- Carbon constraints in like with UK goals of $100g/kWh$ and $50g/kWh$ 
- There is also a security constraints based on the LOLP (which is a function of the capacity/peak demand)

Further, the investment cost for heat infrastructure and distribution network reinforcement costs is calculated through the fractal method. This takes in the number of consumers and heat demand in representative district through the UK heat demand map, which used to establish the topologies and length of the representative network.
- This minimises error in heat demand, number of households and geographical areas.

Further, the paper also suggest that the electricity generation profile can be changed (varying the amount of gas generation (it would be interesting to model this over the retiring coal fired power plants and do an integrated planning scenario like that)). It should be noted that the paper follows GB renewable targets with fixed volumes of wind, solar, and nuclear.

Investigated two scenarios
- slow transition (grid is $100\frac{gCO_2e}{kWH}$)
- fast transition (grid is $50\frac{gCO_2e}{kWH}$)
## Results
The figure below shows that integrated planning (including the electricity power system in the system boundary), has the following effects
- The reduced OPEX is due to more efficient CHP and mitigation of renewable curtailment
- The use of hybrid gas boilers reduces peak load on the heat distribution network and electricity network
- There is additional CAPEX for end use TES, industrial heat pumps and industrial gas boilers.

Essentially, the heating network gives more flexibility to the electricity system (particularly through ancillary services and preheating). ~={green}The model temporarily turns down heat pumps (outlining that this does not affect the thermal comfort of the user), however, it is unclear if this can be done for industrial loads.=~ 

Further, the diagram below shows that there is a correlation between the carbon constraint and the system configuration. Additional simulation highlights that when the carbon constraint exceed 266g/kWh, it is no longer influenced by the carbon constraint.

![[Screenshot 2026-10-06 at 8.54.16 am.png|351]]

Integrated design reduces the need for CCGT and NG CCS, due to the lower VRE curtailment, which therefore reduces the system costs.
#### Heat network

Heat networks are applied in urban areas, and hybrid heat pump gas boilers (end use) are used in suburban, semirural and rural areas, indicating that heat density is a key driving/limiting factor for the application of a district heating network.

Overall, when integration is enabled, heating technologies shifts from hybrid gas-heat pumps to heating networks.
- This means a higher investment in heating infrastructure
- But there is savings in lower system operating costs associated with the NG CCS

In the slow transition scenario, CHPs generate $21$% of the heat while in the fast transition scenario, CHPs generates $7$% of the heat. This shows that although CHPs are effective at increasing flexibility of the integrated system, it is an emission intensive technology.
- It is also not economical to deploy CHP CCS in the long term, instead CHPs are displaced by industrial heat pumps (which may not be possible at a higher temperature)

TES has a positive impact on the heating network through
- Ancillary services that alleviate the curtailment of VRE
- Reducing NG CCS capacity through ancillary services that alleviate VRE
- Shifting heat delivery from end use to district based
However, the paper does not discuss the topology and sizing of the TES and how that
#### Electricity network impacts

Overall, the emissions from the electricity network will increase due to increased operation of NG CHP to fulfill electricity demands. (In the decoupled case, missing generation from the curtailment of VRE is supplied by NG CCS)
## Limitations

However, network topology are approximated through the ~={red}fractal method=~ and the paper only considers the use of hybrid gas boilers + ASHP at the end user, WSHP, GB at the district heating level.
- The analysis is also too wide-pan and does not dive into system/network topology. 
- Further, there are limited technology options in this paper, as end consumers are constrained to using hybrid heat pump gas boilers and district heating networks are constrained to either gas boilers or heat pumps.

Curtailment is not solely based on demand, but also due to thermal constraints in the grid.

Incorporates weather data but does not examine how the network performs under stressful weather conditions. Therefore, does not examine performance of the network under different weather conditions

Only shows monetary impact of improving flexibility of the system. What are the actual impacts on system strength and power grid resilience?

Again, this study is exclusively for commercial heat demand, and does not discuss impacts on industry. It is important to consider heat loads of different temperature requirements, which will change how the heating network look like dramatically. 



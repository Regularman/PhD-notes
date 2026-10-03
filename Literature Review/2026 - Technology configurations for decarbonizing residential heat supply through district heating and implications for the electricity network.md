https://www.sciencedirect.com/science/article/pii/S2589004226020870
## Contribution 

Uses MGA (Modelling to Generate Alternatives) to find near cost-optimums (CAPEX+OPEX) designs for district heating networks, most notably, the spatial distribution and selection of different technologies. The study answers the following questions

1. What is the range of alternative, economically comparable technology configurations for decarbonizing DHNs, and to what extent do these configurations differ in their electricity network impacts?
2. What trade-offs are involved when the deployment of certain low-carbon heat supply technologies is constrained by local conditions, and what are the spillover effects on the electricity network?

The MGA framework uses endogenous load profiles calculated from the least cost or near least cost HPN solution, then combines with exogenous on other load profiles to calculate an AC power flow simulation. This gives information on line loadings and transformer loadings in the network. The study simulates the Dutch region of South Holland. They focus on one of its largest existing DHNs, which is projected to expand substantially in the future, reaching an annual heat demand of about 2,700 GWh and a peak capacity of 1,400 MW by 2050.
- There are around 3605 near cost optimal solutions, each of which is subjected to a full years of AC power flow simulation given load profiles.
![[Screenshot 2026-10-03 at 8.07.50 pm.png|413]]
#### The problem with cost-minimised heating networks
Does not model intangible dimensions such as social acceptance, ~={green}system resilience=~, structural uncertainty.
- For example, while residual waste heat from industry is a cheap way of meeting residential heating demands, it may be unreliable and is not exactly long term (factories can move away or operations can change)
- This means that least cost solutions often have an over-reliance on large capacities of technology and over-deployment of a technology in a single location

#### Metrics used
![[Screenshot 2026-10-03 at 8.46.00 pm.png]]
## Results

The results section will outline the tradeoffs found using this study in Holland. There are a lot of solutions and each technology utilisation can go to $0$. The fact that all technology configurations can be made redundant in different SPORES (district heating configurations), means that different technologies can be traded off together whilst maintaining near cost optima. 

To obtain new decarbonised heating configurations, certain technologies are constrained, and other technologies increase in capacity to compensate. Within the near-optimal decision space, almost all technologies can be fully substituted by functionally equivalent alternatives, and thus are ‘‘real choices’
- Reducing green gas boilers from 400 to 100MW increases the deployment of hydrogen (+240MW) and electric boilers (+100MW). This reduces the need for storage due to additional peaking capacity.
- Reducing electric boilers is displaced by higher heat pump (+160MW) and hydrogen boiler (+200MW) capacities. Further, there is more thermal storage to exploit low price periods in electricity and hydrogen, which is more volatile than green gas
- Reducing residual heat from 200MW to 90MW is compensated by higher waste to energy (+200MW) and geothermal energy (+5MW) as well as higher pipeline expansion (+255MW) to connect there remote heat sources

#### Cost optimal solution
The cost optimal solution relies primarily on green gas and electric boilers. (green gas refers to biogas that has been upgraded to natural gas quality such that it can be directly injected into the national gas grid) 

Half of the heating demand is also provided for a petrochemical company in Rotterdam, which may not always be avaliable in the future.

- Note the use electric boilers, which are less energy efficient than heat pumps (due to lower COPs), but involves a lower CAPEX and OPEX (~={red}the model does not step through the LCOH of each technology=~). Furthermore, the electric boilers are near the demand centre to minimise heat network expansion costs
![[Screenshot 2026-10-03 at 8.19.21 pm.png|269]]

#### Low electrification scenario

Interesting, when there are a higher share of gas boilers (+70%) and an increase in pipeline capacity (+265MW), the level of electric loading on the power grid actually increased. This is as the local PV generation flowed upstream, causing reverse power flow and overloading on the transformers.
#### High and highest electrification scenarios

Higher integration of P2H technologies actually decreases grid loading due to intelligent distributed build outs of heat pumps with thermal storage rather than electric boilers.
- Therefore, spatial deployment is an extremely important factor, in addition to technology choices.

#### Climate sensitivity

Only performed for cold weather year, which has high demand. In this scenario, CHP deployment only increased slightly, as there were not enough periods of high electricity demands to warrant extensive deployments of CHP.

#### When constraining baseloads (geothermal and residual heat)
 Displaced by either carbon neutral gas boilers or intelligently deployed heat pumps coupled with thermal storage.
## Limitations and assumptions made

Does not consider growth in the network. How easy is it to expand capacity of the heating network? If a new factory was going to be built next door, in the same neighbourhood? What metrics or modelling methods are available to do so?

Loading on the power network is just one consideration of the grid operator, what about other grid qualities such as system strength, resilience to climate change, and demand response.
- When talking about resilience to grid events, it would be interesting to model extreme climate events or grid events and analyse response of the heating network, and vice versa, what will happen to the electricity network when a portion of the network just shuts of suddenly.

Further, the study is making the assumption that everyone is connected to the HPNs. It does not consider load profile compatibilities.
Does not answer the question of what characteristics drive certain decision variables within the heat production network design.

Further, how will these technology options look like when considering the GWP and other sustainability metrics of the HPN?
- Further, the study does not map the ex-ante to ex-post strategies to decarbonise the heat supply. For example, whether the system should rely on heat electrification to absorb excess generation from PVs or should the generation be directly curtailed.
- Additionally, the study only analyses the current state of technology options. Does not consider improvements in technologies in the future.

The study only considers the design of 4GDH, and does not include the cooling needs of the local region.
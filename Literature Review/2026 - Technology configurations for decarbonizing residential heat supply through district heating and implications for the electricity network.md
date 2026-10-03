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

#### Metrics used
## Results

The results section will outline the tradeoffs found using this study in Holland. There are a lot of solutions and each technology utilisation can go to $0$. The fact that all technology configurations can be made redundant in different SPORES (district heating configurations), means that different technologies can be traded off together whilst maintaining near cost optima. 

To obtain new decarbonised heating configurations, certain technologies are constrained, and other technologies increase in capacity to compensate.
- Reducing green gas boilers from 400 to 100MW increases the deployment of hydrogen (+240MW) and electric boilers (+100MW). This reduces the need for storage due to additional peaking capacity.
- Reducing electric boilers is displaced by higher heat pump (+160MW) and hydrogen boiler (+200MW) capacities. Further, there is more thermal storage to exploit low price periods in electricity and hydrogen, which is more volatile than green gas
- Reducing residual heat from 200MW to 90MW is compensated by higher waste to energy (+200MW) and geothermal energy (+5MW) as well as higher pipeline expansion (+255MW) to connect there remote heat sources

#### Cost optimal solution

The cost optimal solution relies primarily on green gas and electric boilers. (green gas refers to biogas that has been upgraded to natural gas quality such that it can be directly injected into the national gas grid) 

Half of the heating demand is also provided for a petrochemical company in Rotterdam, which may not always be avaliable in the future.

- Note the use electric boilers, which are less energy efficient than heat pumps (due to lower COPs), but involves a lower CAPEX and OPEX (~={red}the model does not step through the LCOH of each technology=~). Furthermore, the electric boilers are near the demand centre to minimise heat network expansion costs
![[Screenshot 2026-10-03 at 8.19.21 pm.png|269]]
## Limitations and assumptions made

Does not consider growth in the network. How easy is it to expand capacity of the heating network? If a new factory was going to be built next door, in the same neighbourhood?
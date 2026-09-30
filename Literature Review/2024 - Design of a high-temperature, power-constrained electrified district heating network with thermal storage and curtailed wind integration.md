https://www.sciencedirect.com/science/article/pii/S221313882400211X

## Contribution

Looks at the design of heat production network from both the grid operator and end user perspective. This is considered in terms of 
- lower wind energy curtailment
- grid constraints of grid connection at the University of Edinburgh

Currently, KB in the University of Edinburgh is a large campus which currently operates a 2.7 MWe CHP unit together with three 7 MWth gas boilers coupled with a 150 m3 hot water thermal buffer tank to meet its thermal demand.
- There are a lot of historic buildings and an existing high temperature district heating network ($85\degree C$). Upgrading these to a low temperature district heating network will require extensive retrofits and therefore has not been considered in this study.

The proposed electrification system is set, and rather wind curtailment is achieved through ex-post control strategies
![[Screenshot 2026-09-29 at 3.28.42 pm.png|700]]

In this system, the BTES is charged from a TES (because of the low charging rate of the BTES), and the TES will act as a buffer for the air source heat pump.
- This TES system also is used to increase the temperature of the district heating network for the supply line.

The BTES system stores energy from the air source heat pump during the summer and releases this energy into the return line during winter. Releasing heat back into the return line means that the temperature of the TES will have to be higher, increasing standing heat loss.
## Content

The study looks at the ex-post control strategies that can be used to to mitigate wind curtailment.

| Control strategy | Description                                                                                                                                                                                                                                                                                                                                                                    |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Demand regime    | The control strategy dictates that the air source heat pump will operate (in the case of non-wind curtailment, following demand of the load in the University of Edinburgh). If wind curtailment occur, then the TES will charge to full capacity and discharge until it is empty.                                                                                             |
| Baseload regime  | The control strategy dictates that the air source heat pump will operate (in the case of non-wind curtailment, the air source heat pump will act to baseloads. If the baseload is insufficient to address demand, then either discharge from the TES or raise baseload.  If wind curtailment occur, then the TES will charge to full capacity and discharge until it is empty. |
| COP regime       | The control strategy dictates that the air source heat pump will operate (in the case of non-wind curtailment, the air source heat pump will act to baseloads only during hot hours to maximise COP of heat pump).   If wind curtailment occur, then the TES will charge to full capacity and discharge until it is empty.                                                     |
After consideration of wind curtailment rate, which starts at 17.21%, the metric can be translated into grid CO2 emission intensity factor and retail price of electricity.

Model simulation done in TRNSYS under 324 different scenarios.
- Note that the BTES is discharged whenever it has a higher temperature than the return line, given a buffer of $2\degree C$.

### Results

There is a conflicting variable of interest in this case study. 
- The grid operator wants as little wind curtailment as possible and therefore higher electricity consumption from the industry is favourable. However, this means that inefficient use of electricity is rewarded, which reduces the financial case for the industry/end consumer.
#### Load leveling

The utilisation of curtailed wind energy reduces the flexible loading capacity of the system. This is as the heaters and heat pumps must run at full capacity during any wind curtailment events, which can happen during any time of the day and season.

By taking the season averaged profiles, the study highlights that control strategy 3 as having the highest variability, due to the limited size of the TES, which does not allow the heat demand during the hottest part of the day to be carried over to the evening demand periods.

![[Screenshot 2026-09-30 at 4.55.19 pm.png]]

Overall, the results highlighted that the control strategy is the best for managing flexible electrical demand, although this requires knowledge of next day's demand, and the study does not quantify the impacts of black swan events on the heating system.
#### Mitigating Wind Curtailment

 As wind curtailment increases, the temperature of the battery storage will increase. This will increase the COP of the heat pump, which means that the electricity consumption at air source heat pump must decrease to maintain a steady outlet temperature. This means that the excess electricity must be absorbed by the electric boiler to ensure that the electricity is used, reducing the thermal efficiency of the system.

- This trade-off shows the differing interests of the grid operator and end consumer, which can be rectified through cost recovery schemes. There needs to be market incentives for the uptake of wind.

From simulation data, control strategy two is the best at reducing wind curtailment by ensuring that the system can take as much of the curtailed wind as possible, constrained only by the TES size and the charging rate.
- The size of the TES is determined by the supply temperature $70\degree C$.
#### Effect of the supply temperature

- As the supply temperature decreases, and the air source condenser outlet temperature remains the same, then the wind integration factor increases. A lower supply temperature means a less heat loss and a higher thermal energy efficiency.
## Limitation

The study does not consider an waste heat recovery, which is crucial to heat network operation. 
- Furthermore, the study does not consider the topography of the heating network in the optimisation of the selected metrics

TES discharge strategy is not time dependent, a demand following TES should be used to minimise cost for the users.

The shape of the curtailment events will also the matter. How has wind curtailment change over the past 10 years?

Industry requires steam, how does this fit in with the rest of the load profiles.

Metrics were not quantified by all the variables, which limits commentary which can be done for the energy system. Furthermore, the commentary is only specific to this one system, and does not inform network topography design.
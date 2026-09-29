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
- The grid operator wants as little wind curtailment as possible and therefore higher electricity consumption from the industry is favourable. However, this means that inefficient use of electricity is rew

## Limitation

The study does not consider an waste heat recovery, which is crucial to heat network operation. 
- Furthermore, the study does not consider the topography of the heating network in the optimisation of the selected metrics

TES discharge strategy is not time dependent, a demand following TES should be used to minimise cost for the users.

The shape of the curtailment events will also the matter. How has wind curtailment change over the past 10 years?
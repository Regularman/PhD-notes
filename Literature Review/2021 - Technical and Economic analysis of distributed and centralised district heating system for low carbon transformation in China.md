
https://ieeexplore-ieee-org.wwwproxy1.library.unsw.edu.au/stamp/stamp.jsp?tp=&arnumber=9736089

## Contributions

Reviews current studies in distributed versus region level district heating. The paper then proposes a comparison of district heating substation ($SG > 20000$) and building wise substation ($20000 \ge SG \ge 1000$) and household wise heating stations  ($1000>SG$) in terms of 
- economic
- energy
- carbon emissions
Under a range of heating areas based on 2 real heating systems in Northern China

This idea of system sizing is termed Substation Granularity (SG) $$SG=\frac{\text{Total Heating Area}}{\text{Heating Substation Area}}$$
## Content

Annual cost is lower in selected case under BHS compared to CDHS.

- CDHS transfers high temperature hot water of heat source to teh DHS through a primary network to heating substation, then to terminal users through a secondary network (soviet).
- BHS is more nordic. The primary network connects directly to intelligent buildings and heats the users through heat exchange substations
- HHS is one heating substation per household, used predominantly in Germany and Denmark

~={red}To find the temperature of any node in the heating network, we can use the equation provided in the paper, which is sourced from [22]. =~Note that the temperature of each node is is dependent on the surface heat dissipation coefficient of the radiator, which changes based on temperature. This needs to be solved iteratively.

To assess the feasibility of each scale of solution, the paper uses three indices,

| Index              | Method                 | Details                                                                                                                                                                                                                                                                                                                                                                             |
| ------------------ | ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Economic           | Annual cost method     | $C_a = \alpha C_{in} + C_{run}$, where the investment coefficient is determined by the internal recovery ratio, set to 0.1. $$\alpha = \frac{I(1+I)^n}{(1+I)^n-1}$$The project lifecycle $n$ is 15 years.                                                                                                                                                                           |
| Energy consumption |                        | Splits into the heat consumption, power consumption, and water consumption index calculated in (consumption/$m^2$). Heat loss is related to heat dissipation and hydraulic imbalance of the pipe network. Water consumption is related to the water supplement level and the circulating flow of the pipe netowrk. Power consumption is related to circulating water and pump head. |
| Carbon emission    | Bottom up LCA approach | Built from bottom up using life cycle inventory analysis. Uses coal as the default fuel for energy supply, rather than any other renewable options.                                                                                                                                                                                                                                 |
The index base price of heating area for CDHS is based on [19]. While BHS is only based on the equipment costa and is area agnostic.

Hydraulic imbalance occurs when the heating area of a single heating substation is too big. This is caused by irregular flow within the network, and has always been a major factor in heating energy consumption. This can be fixed by 
- Increasing the flow of heating,
- improve average temperature of overall supply and return
- Improve heat consumption and power consumption
The paper models hydraulic imbalance as a function of the SG, but how do you quantify the actual level of ~={orange}hydraulic imbalance=~ in the system?

The cities and provinces they chose were 10-18.5$\degree$C below $0$.

|                          | Hebei                 | Heilongjiang      |
| ------------------------ | --------------------- | ----------------- |
| Temperature              | $-10\degree C$        | $-18.5 \degree C$ |
| Heating area             | $1.5 \times 10^5 m^2$ | $1.8 \times 10^5$ |
| Length of heating season | 120 days              | 180 days          |
Ultimately showed that BHS has a lower consumption index compared to centralised district heating systems. However, this does not account for the pipe netwo
## Question

1. ~={green}Would be interesting to also look at base case (do nothing), district heating, and centralised heating.=~
2. Over the past decade, Chinese district heating has grown by 13% p.a, reaching 11 billion square meters by the end of 2019.
	- ~={green}What has the impact of this been? =~Paper cited problems with low heating efficiency, high hydraulic imbalance rate, and serious heat waste. This is compounded by complex pipelines, serious water loss, and high power consumption
3. What is the difference between 4th and 5th generation district heating and cooling systems?
4. ~={green}How does different heating behaviour affect the system?=~

## Limitation

1. Uses coal as the main fuel source.
2. Does not consider the length of the pipe network to be a consideration.

## Further Readings

[3] [4] Look at these papers for district cooling and smart thermal grids.
[6] ~={red}DER design method based on linear programming for the design and evaluation of a bi-di low temperature network. This model optimises cost while selecting the optimal area and selection for the building and energy hub=~
[10] might serve to answer some questions about operational inefficiencies in Chinese DHS
[12] used smart meter data for unsupervised learning of energy signals to identify heating systems and building types.
[15] ~={red}Very relevant to decentralised heat networks. Talks bout multi-heat source ring network and how to reasonable design the location of the pipe networks, heat sources, and how to reasonably connect the heat system using grid analysis method=~
[16] Heat source location on system economy of a district heating network


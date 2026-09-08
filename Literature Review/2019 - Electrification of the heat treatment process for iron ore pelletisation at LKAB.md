https://odr.chalmers.se/server/api/core/bitstreams/f2234f8d-4c1f-4bec-b6ea-f4978d7c98af/content
## Contributions

LKAB mines 80% of EU ores. In 2017, LKAB produced over 27.2 million ton iron ore products and iron ore pellets accounted for around 83 % of LKAB’s iron ore deliveries.

This report will focus on the heat treatment of the pellets (in grate kilns and straight grate processes)
- The grate kiln uses a travelling gate for drying, preheating, and cooling and a kiln for sintering (best for magnetite). it uses convective heat transfer between the heated gas and the iron ore pellets. It is best for magnetite because hematite produces more fines when mixed in the rotating kiln and has higher radiative loss.
- While the grate kiln process receives an important contribution to the heat treatment via radiation from an open flame.
- The straight grate uses a travelling gate for all 4 steps (handle ores with higher hematite content and can achieve a lower fuel consumption).

Currently, heat is produced form fossil fuel to get the pellets up to temperature. The oxidation of the iron ore also produces heat.

Interest in replacing fossil fuel burner with microwaves and plasma torches
- One issue is that this might affect the quality of the iron pellets
- And high temperature of the plasma creates NOX. This is studied through reaction modelling in Chemkin

The report will look at how high temperature heat can be supplied by plasma torches in the straight grate process
- And where microwabes can provide low temperature heat input to the straight grate process
- Investigate emission impacts of electrification
- Optimisation opportunities of electrification

This study will focus on the straight-grate process due to its adaptability to plasma heating.
## Content

In the LKAB mines, magnetite with iron content of 80-100% are mined.
- The iron ore leaves the sorting process with an iron content of 45% and leaves with 62% by filtering out waste rock. And then to 68% when it's grounded and formed into a slurry.
- With the help of a binder named bentonite, the pellets can be sintered so they withstand the stress of transportation to the steel making plant.
	- The iron ore, with bentonite needs to be dried and preheated, sintered, and then cooled.
- Furthermore, another reason is that the uniform spherical shape allows even gas flow around the pellets, allowing for better reduction

Note that is should be easier to replace the straight-grate process because replacement of the open flame with plasma fires will have different heat properties.

In considering sintering there are four reactions


| Reaction                                                                                                                                                                                                                                           | Formula                                  | Enthalpy change ($kJ/kg$) |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- | ------------------------- |
| Evaporation - from 9% wt% to 0%                                                                                                                                                                                                                    |                                          | 2256                      |
| Oxidation - However, the sintering of hematite will not have this exothermic reaction. Reaches maximum conversion efficiency at $1100\degree C$. If the temperature exceeds $1300\degree C$ then the hematite will disassociate back to magnetite. | $$4Fe_3O_4+O_2\rightarrow6Fe_2O_3$$      | -119 $kJ/mol$             |
| Calcination from the limestone additives. But there is relatively little limestone and therefore little heat demand. Occurs from 600-900$\degree C$                                                                                                | $$CaCO_3\rightarrow CaO+ CO_2$$          | 182 $kJ/mol$              |
| Decomposition of dolomite. Low heat demand due to low concentration.                                                                                                                                                                               | $$CaMg(CO)_3\rightarrow CaO+MgO +2CO_2$$ | 296$kJ/mol$               |

![[Screenshot 2026-09-08 140541.png]]
### Drying

This occurs by blowing post process gas into the unprocessed iron ore in the UDD and DDD zone. The drying is switched from updraft to downdraft to achieve a more homogenous evaporation rate and reduce the risk of recondensation of water in the bottom layer.
- The drying can't be too fast or the pellets will crack

## Sintering

During the preheating and sintering phase, the particles in the pellets diffuse and partly fuse together, increasing their mechanical strength. The oxidation of magnetite into hematite occur simultaneously.
- Approximately 60% of the thermal demand comes from the oxidation of magnetite into haematite. The majority of this oxidation occurs in the firing and after firing zone.
	- Note that gas is reused from the cooling zone and heated to $1100-1300\degree C$.
	- In the current MK3 unit, 4 natural gas burners and 12 oil burners are used for the additional energy supply.

In a grate kiln, the rotating drum spreads the heat evenly and the heat is provided by a direct fire (fueled by coal). 
### Cooling

The products are then cooled down to below $100\degree C$.

## Electrification solutions

### Microwaves

Microwaves have been shown to heat up metal powders, but not when presented in bulk. Material properties affect whether the particles transmit, reflect, or absorb the microwave radiation.
- Electrons will become concentrated at the surface and arc if the metallic surface is reflective of microwaves

Magnetite and hematite shows good absorption of microwaves. The water in the microwave are also good absorber of water.
- However arcing has been observed at high temperature

Microwave causes more rapid heating as the heat does not diffuse from the surface, but happens from within. This means that non-homogenous materials can heat unevenly. The heat distribution depends on the dielectric and conductive properties of the materials.
- This is governed by the di-electric properties and polarity of the material. Polar molecules will oscillate under the presence of an EM field, and the thermal energy spread throughout the material, driven by thermal gradients.
- This can cause thermal runawat, and crack the iron pellets.
- Heating is also caused by the movement of electrons in the metallic lattice

In early 2018, there was a study published by Athayde et al. [23] investigating kinetic parameters of the iron ore pellet drying process assisted by microwave technology. In this study, green pellets were produced from hematite ore and sieved into three size categories with average diameters of 10.75, 13.5 and 15.25 mm having a moisture content of 10 %. Samples of 100 g were subjected to microwave radiation for 180 s with intervals of 30 s using a turnable-tray microwave oven normally used for heating food. The frequency used was 2.45 GHz and the power levels used were 300, 600 and 1000 W. The tests were conducted at temperatures lower than 500 °C.
- 


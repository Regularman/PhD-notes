https://odr.chalmers.se/server/api/core/bitstreams/f2234f8d-4c1f-4bec-b6ea-f4978d7c98af/content

Sintering takes between 1.26 (global best)-2.55 GJ/t sinter for Indian sources. [Source](https://www.sciencedirect.com/topics/engineering/sinter-machine)
While US sources highlights that it is around 1.5-1.7Gj/t-product. [Source](https://www.osti.gov/servlets/purl/1026806)

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


| Reaction                                                                                                                                                                                                                                           | Formula                                  | Enthalpy change ($kJ/kg$)                                                                                                                                                                |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Evaporation - from 9% wt% to 0%                                                                                                                                                                                                                    |                                          | 2256                                                                                                                                                                                     |
| Oxidation - However, the sintering of hematite will not have this exothermic reaction. Reaches maximum conversion efficiency at $1100\degree C$. If the temperature exceeds $1300\degree C$ then the hematite will disassociate back to magnetite. | $$4Fe_3O_4+O_2\rightarrow6Fe_2O_3$$      | -119 $kJ/mol$ of magnetite. Since the molar mass of magnetite is $231.53 g/mol$, the enthalpy of heat is $513.97kJ/kg$. This translates to$ $0.513GJ/t$ of sinter. This provides around. |
| Calcination from the limestone additives. But there is relatively little limestone and therefore little heat demand. Occurs from 600-900$\degree C$                                                                                                | $$CaCO_3\rightarrow CaO+ CO_2$$          | 182 $kJ/mol$                                                                                                                                                                             |
| Decomposition of dolomite. Low heat demand due to low concentration.                                                                                                                                                                               | $$CaMg(CO)_3\rightarrow CaO+MgO +2CO_2$$ | 296$kJ/mol$                                                                                                                                                                              |

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
- This can cause thermal runaway, and crack the iron pellets as well as the reduction of hematite back to magnetite. Thermal runaway is difficult to detect as it is internal
- Heating is also caused by the movement of electrons in the metallic lattice

However, this method does not displace fossil fuel because drying gas is from the waste heat form the cooling region anyways.
- From test 1 and 2 below, microwaves could be used in the updraft zone to eliminate the recondensation of moisture in the higher layers by heating the bed from both sides i.e. convective heating from below and microwave heating from above.
- This will shorten the drying time and lead to increased production rate and higher quality end product
#### Test 1 - purely microwave

In early 2018, there was a study published by Athayde et al. [23] investigating kinetic parameters of the iron ore pellet drying process assisted by microwave technology. In this study, green pellets were produced from hematite ore and sieved into three size categories with average diameters of 10.75, 13.5 and 15.25 mm having a moisture content of 10 %. Samples of 100 g were subjected to microwave radiation for 180 s with intervals of 30 s using a turnable-tray microwave oven normally used for heating food. The frequency used was 2.45 GHz and the power levels used were 300, 600 and 1000 W. The tests were conducted at temperatures lower than 500 °C.
- When drying the pellets, an intense heating rate was observed in the beginning of the drying phase. The heating rate slowed down as the moisture content of the pellets decreased which indicates that the moisture content is an important parameter for the ability of the pellets to absorb microwave energy. 
- The dryout time was slower in small pellets than in large pellets. This was likely due to the large surface area to volume ratio which leads to large heat loss to the surroundings.
- Effects on pellet quality was assessed by evaluating the crushing strength of the pellets after drying with microwaves. Results showed strength levels varying between 0.6-2.5 kg/pellet which is considerably lower than conventional methods.

#### Test 2 - combined convection and microwave

The effect of combining microwaves and traditional convective heating was evaluated against the traditional processing technique using only convective heating. The UDD mode introduced an airflow with an inlet temperature of 290 °C during 175 seconds before switching to the DDD mode which introduced an airflow with an inlet temperature of 280 °C during 340 seconds. The microwaves were used only during the UDD operation mode at a frequency of 915 MHz and a constant power supply of 10 kW. Green pellets were produced using iron ore dominated by hematite mineral. The majority of the pellets had a diameter between 9-16 mm. The moisture content was adjusted to batches of 10 % and 10.3 %

The surface layers of the pellet bed showed considerably higher temperatures when using microwaves. At 60 mm depth the temperature reached 115 °C compared to 71 °C in the purely convective case.
- Results from moisture measurements in different levels of the bed at the end of the UDD section showed that purely convective flow increased the moisture content in the upper layers of the bed by 0.08 - 0.36% compared to initial levels due to recondensation of moisture. The microwave assisted drying process decreased the moisture content in the higher layers by 0.12 - 0.8% compared to initial levels, which was a considerable improvement.

### Plasma torches

Plasma is when the material gets so hot that the electrons leave it and we get a positively charges gas. The high temperature in combination high reactivity translates to a high heat transfer rate and chemical reactions.

- Thermal plasmas with low degree of ionisation and equal temperature of ionised gas and electrons
![[Screenshot 2026-09-08 152650.png]]

These devices work by creating an electric arc between a cathode and an anode using a DC current, which is more stable and easy to control compared to AC. 
- The working gas is pumped along the outer boundary of the gun to cool the boundary layer in a vortex or linear flow to guide the plasma jet. The working gas can be argon, hydrogen, nitrogen, helium and air. If high energy content are desirable, use diatomic particles due to disassociation reactions before ionisation. If inert environment is required, use argon, and reactive gases like H2, O2, and N2 can be used to provide reducing or oxidising effects.
- When the ionised gas leaves the gun, it returns to its non-ionised state, but is still superheated
- Electrothermal efficiency of 50-70%, but 90% have been observed.
- Industrial applications of up to 8MW.
- Can burn between 5000 to 30000K.
- A non-transferred plasma torch has the anode inside the gun. The example above is non-transferred.

|                                    | Fuel oil burner                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Plasma gun                                |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------- |
| Thermal capacity                   | 2 MW                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | 2MW                                       |
| Annual Electricity consumption     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | 20 GWh                                    |
| Power                              | 17.52 MWh                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | 17.52 MWh                                 |
| Power required per tonne of sinter | $1.29GJ/t$. See above. However, LKAB states that they have reduced fuel consumption to $8L/t$, which is around $0.308GJ/t$.                                                                                                                                                                                                                                                                                                                                                                            | $1.29GJ/t$. See above.                    |
| Sinter to DRI efficiency           | $1.5t$                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |                                           |
| Carbon emissions                   | $222.525 kgCO2-eq/t-CS$. note that this is consistent with [[2017 - Power-to-Steel - Reducing CO2 through the integration of Renewable Energy and Hydrogen into the German Steel Industry]], which states that sintering releases approximately $271kg/t-CS$. However, note that in this paper, LKAB states that they have reduced carbon emissions to around $31kgCO2-e/t$. [[2020 - Toward a Fossil Free Future with HYBRIT - Development of Iron and Steelmaking Technology in Sweden and Finland]] | Potentially 0 with renewable electricity. |
#### Applications of plasma torch

![[Screenshot 2026-09-08 155620.png]]

- Are there energy savings when using hydrogen or oxygen as a plasma gas due to the oxidation or reduction that occurs?
- The heating of process gas with electricity rather than combustion will produce less water vapour within the process gas that is used for drying, which is good. However, the effect of this is not discussed in the paper
- High temperatures of the plasma gas can lead to undesirable effects such as NOx generation caused by the formation of thermal NOX gas. NOX gas can cause acid deposition through acid rain and formation of tropospheric ozone. This is as NOX gas decompose in sunlight to create oxygen free radicals that creates ozone.
	- There are three ways to create NO; thermal NO from high temperatures, fuel NO from oxidation of nitrogen in fuel with oxygen in air, and prompt NO from the nitrogen in air and hydrocarbon radicals in fuel. Thermal NO can be described by the Zeldovich equations $$\begin{align} N_2+O&\leftrightarrow NO+N \\ N+O_2&\leftrightarrow NO+O\\ N+OH &\leftrightarrow NO + H \end{align}$$We can avoid thermal NOX by decreasing oxygen concentration and reducing thermal peaks, as well as balancing the equilibrium and gas residence time. 

- Lack of mixing in the design causes thermal stresses and uneven oxidation of the pellets.
## Bedsim model

Validated against lab scale tests as a model of the straight grate and grate kiln processes.
- The model performs calculations for chemical reactions as well as mass and heat transfer between the process gas and the bed. 
![[Screenshot 2026-09-09 at 12.26.06 am.png|545]]
- Note that LKAB MK3 straight grate uses 5L of oil per ton of finished pellet. Since the density of is around $750-850 \frac{kg}{m^3}$, and the energy content is ~$38.6\frac{MJ}{L}$, then the energy requirement is around $193\frac{MJ}{t}$. This 

- The main goal of the simulation model is to calculate the NOX formation of the plasma gun case using a reactor model, as well as the degree of oxidation from magnetite into hematite, the gas temperature throughout the grate, and the pellet temperature (which is important to control the oxidation reactions).

![[Screenshot 2026-09-09 at 12.24.09 am.png]]
- However, more important attributes of pellet strength and deformation could not be simulated in the model, which only looks at mass and energy balance. 
- Thermal runaway, heating rate, crushing strength of the pellets and decreased pellet deformation and clogging cannot be measured with the simulation model and therefore these must be analysed in practical tests.
- Furthermore, too high temperatures can lead to difficult handling of the sinter at the end
- The calculations do not include the thermal efficiency of the burner
- It is known that BedSim overestimates the temperature from the AF zone as it does not model the leakage of air

The model is validated through comparing with experimental results produced by [25]

![[Screenshot 2026-09-09 at 12.28.57 am.png]]

## Chemkin model for NOX formation

The quantities of NOx produced from a plasma torch can be qualitatively estimated by reaction modelling in Chemkin based on established gas phase reaction kinetics. A common type of reactor model used for combustion modelling is the one-dimensional plug flow reactor (PFR). In the PFR a temperature profile can be defined and the reactions are calculated at different distances from the reactor inlet.
- Since many parameters of the torches are unknown, the study is of a qualitative nature instead of a quantitative
- Meant to be a guideline for choosing plasma torches

Looked at three cases
- NOMIX - which does not consider mixing with gas and only considers the NOX formation from the hot plasma
- MixTP - which considers the temperature of the gas to the same as the reference case
- MixEE - Which calculates using energy balance, the temperature of the mixed air as you move down the grate. 

In the case where there is air mixing, the reaction area increases linearly from the outlet of the AF section to the outlet of the cooling section. Note that this study does not consider the dependency between outlet diameter and the amount of mixing air, which affects the gas residence time.

Validated against Cementa testing results [41].
- Considered two methods of NO reduction
	- Re-burning through mixing with methane to destroy NO through hydrocarbon radicals
	- Reduction of oxygen content in the mixing air with combustion (complete combustion with methane)

## Implementation of microwaves - simulation results

Ultimately showed that there was no decrease in fossil fuel use, as most of the microwave is being carried out by the process gas flow. The temperature of the gas flow leaving the UDD zone would likely be around, or even below, 100 °C assuming that it reaches approximately the same temperature as the pellets in the top layer of the bed. This is low-grade heat which has limited application areas.

![[Screenshot 2026-09-09 084955.png]]

This means that the fossil fuel usage decreased by 0.398%. This must be assuming they process around 450.89 tph. To combat this, the paper suggested alternative design. This can be done by altering the grate area in the cooling and UDD zone. By optimising these parameters, it was possible to slightly displace the high temperature heat with low temperature microwave.![[Screenshot 2026-09-09 085807.png]]

## Plasma gun

The use of plasma torches can completely displace fossil fuel. Also note that the flow rate of the plasma gun is low relative to the air flow in the work grate.

- Also showed improvement in the magnetite content (lower) in the final product as there is more oxygen in the process gas from the lack of combustion. 
- The maximum magnetite content at the end of the process is 2.28 % for air but decreased even further to 0.60 % for oxygen, which indicates that using oxygen as a working gas is a good choice. However, using oxygen increases the grate temperature above the constraint. Using oxygen as a working gas is more expensive but prevents the formation of NOX compared to air as a working gas.

![[Screenshot 2026-09-09 091915.png]]

#### Optimisation of plasma torch process

We can lower the mass flow of process gas to reduce the energy consumption, but this will lower the magnetite conversion rate. Subsequently, to get the same quality of pellets as the reference case, power consumption can drop by 18%.
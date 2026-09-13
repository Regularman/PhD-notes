https://cordis.europa.eu/project/id/768788/results

SIDERWIN technology can contribute to future carbon neutral steelmaking with almost no direct $CO_2$ emissions and $60\%$ less carbon footprint compared to the BF BOF process.

From the pilot trial, the cathode has been scaled up to $1.25m^2$
- Also found that decreasing the solid concentration in the electrolyte is helping gas management without degrading the faradaic yield
- Electrolyte flow uniformity is required to avoid dendrite formation and the following short circuits

Confirmed 2.7MWh of Fe produced are reachable in optimised conditions.

Potential to incorporate mill scales from the steel industry as inputs for circular economy practises.
- However, different compositions of the mill scale will affect the electrochemical cell differently, and more investigation is needed to investigate the percentage that mill scales can be used as substitutes for hematite concentrate in the facility.

## Pilot Technical Performance


| Trial | Description                                                                                                                                                                                | Fixes                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | Based on the ULCOWIN trials, performed in 50 wt% NaOH electrolyte solution with 33wt% of synthetic hematite. Used a graphite cathode and nickel anode leading to fragmented iron products. | Some modifications have then been made on pilot to have a better gas evacuation: opening the evacuation on the top of cell, reducing the electrolyte flow, reducing the hematite concentration from 33 wt. % to 15 wt. % and reducing the current to 1 000 A. These modifications have been tested on 2 trials which lead to less fragmented iron plates, and some further modifications have been made to further improve the gas management. |
| 2     | The first non-fragmented iron plates developed in July 2023. (15kg produced). However, dendrite growths caused short circuits between the electrodes.                                      | Dendrites was reduced by ensuring more uniform electrolyte flow through the cell                                                                                                                                                                                                                                                                                                                                                               |

The average metallic iron content across the different trials was found to be around 96% and can be up to 98.7 % under stable working conditions.
- Based on the weight of the iron plate produced and the assessment of hydrogen produces, was close to 90% under stable working conditions

Showed energy consumptions of 2.7MWh/t under stable operating conditions such as thermal stability, good gas management and uniform and stable electrolute flow.  However, in some trials, this can rise to 7MWh/t due to imperfect conditions.

### Demand flexibility

Reactive power is about 30% of the active power and is satisfactory in comparison to the 40% limit set by France. Correction capacitors can be implemented to reduce the reactive power
- The main electrical consumers, heating elements and electrolyser, implemented at the different stages of the process, are easy to control independently and have an excellent responsiveness to cut-off as the power can drop from full power to 0 in less than 100 ms on request. This level of responsiveness means that this process could, at an industrial scale, be positioned on the most challenging and profitable demand response markets, such as the interruptibility mechanism in France, which requires a maximum delay of 5s.

The heating elements can be split up based on 
- Preparation of the electrolyte
- Introduction and heating of the electrolyte in the loop
- Electrolysis
- Hot rinsing and extraction of the plate
Interruption of the heating elements were maintained in the step 1,2, and 4. Due to the heat loss during the cut off period, these process have a relatively long recovery phase, which increases specific power consumption and increases product cycle duration. However, this was not the case for the electrolyser, where the power and production recovery is almost instantaneous provided that the temperature condition remain stable during the cut-off period.

- Did not evaluate the impact of interruption on the product quality as extended production interruption could not be maintained in the pilot scale facility.

It is recommended that the further development of this technology should consider the thermal integration possibilities with other cells or nearby electric arc furnaces, in order to minimise the power and cost of the electrical equipment and the energy consumption for which heating represents almost 85% at this stage
## LCA - final results

Assuming that renewable energy will have 50% of the demand by 2040 and 70% of the demand by 2050. 

- The functional unit is 1t of HRC and the total steel production in Europe.
- Assumes that iron production is a continuous process with a common 5% interruptions for maintenance and regulatory control. Therefore, the electrical power is 0.33kW/t-iron/year
- 90% of the electrolysis power could be modulated or stopped during a deactivation period.

Considers the use of an induction furnace for the melting of the iron to form hot rolled steel. The total electricity consumption is 4.3MWh/t of HRC.

If the entire steel industry converted to SIDERWIN technology, the grid load per year will be an additional 470TWh, which is the additional electricity demand of France
- The power demand in Europe will be an additional 53.8GW, 42.8GW of which is due to electrolysis
- To best meet this demand, the EU is considering either nuclear or offshore wind technologies. The building of additional generation will also transform the power system, and the direct CO2 emissions of the power system is calculated, along with the cost of the power system and interconnection flows between countries.

To have a full picture of the environmental impact of all assessed technologies, not only climate change impacts are considered but also other indicators such as water use, land use, human health, ecosystem quality and energy demand.

### Results

Note that in the mixed case, we are assuming 2050 scenario of 70% renewable grid, which in the renewable scenario, the grid is 100% decarbonised. In the mixed scenario, the SIDERWIN process is also operating as demand responser operator.

Scope 3 emission consider that other sectors that provide the secondary material source such as iron ore mining and titanium mining, are also decarbonising. Therefore, the emission data may be over-estimated.
- In the mixed scenario, SIDERWIN has 9% more higher water consumption due to evaporated water du to hydropower production. 
- While land use land use for SIDERWIN is 126% higher 
- SIDERWIN has 43% lower human health impact
- 15% lower energy demand compared to BF BOF

However, this study does not count the coal and natural gas that is needed in the EAF or induction furnace stage?
- Assumes that there is not coal or natural gas used, which means that more electrical energy is needed at the induction furnace stage? However, this does not include the natural gas and coal which is inserted into EAF processes and hot rolling processes to accommodate for the fact that the hot charge coming out of the electrochemical cell is very low in carbon. (This may account for the higher electricity comsumption (4.7MWh/t-HRC compared to 3.3MWh in the ULCOWIN paper). [[2016 - Iron production by electrochemical reduction of its oxide for high CO2 mitigation  - ULCOWIN]]
- However, there is a lot of uncertainty around the H-DRI and SIDERWIN data due to a lack of industrial case studies to look at.
- Only focuses on raw material extraction, steel production, and steel recycling. Steel manufacturing and use was too varied to look at.
![[Screenshot 2026-09-13 120159.png]]

In a realistic scenario, SIDERWIN can reduce the carbon footprint of steelmaking to ~0.9kg CO2/tHRC.
- The scope 3 emissions in the SIDERWIN case is ~400kgCO2/t-HRC. This mostly stems from the transportation of beneficiated iron ore, as well as the input of secondary metals for steel property calibration. Therefore, the total scope 1 and 2 emissions, which is what is counted in the APVI spreadsheet, is ~0.1tCO23/t-HRC, which represents ~93% reduction in carbon emissions, down from 1.5tCO2 needed for BF-BOF processes

![[Screenshot 2026-09-13 133721.png|368]]

![[Screenshot 2026-09-13 124351.png]]
- DCAL - Decalcification by Acid Leaching
- LTDA - Low Temperature De-alumination
- UFMI - Ultrafine milling of iron ore
- HTDS - high temperature desilication
- EWIM - Electrowinning of iron metal
- ARME - Acid base regeneration by membrane electronisation
- IMIS - Induction melting of iron metal into steel
- CCOS - Carbon capture and sequestration
- SHRM - Steel hot rolling mill

Note that there is no carbon input into the entire SIDERWIN process. This is compared to the energy and mass balance of H-DRI and BF-BOF.
- It is also assumed that all electricity for the SIDERWIN process comes from hydro-electricity, which is not realistic when considering other impacts
![[Screenshot 2026-09-13 132659.png]]

![[Screenshot 2026-09-13 132805 1.png]]
## Techno-economic analysis

![[Screenshot 2026-09-13 121355.png]]

The market for DSR and grid flexibility is increasing due to the growth of intermittent renewables.

Economic results show that SIDERWIN has the potential to be profitable form 2030 onwards.
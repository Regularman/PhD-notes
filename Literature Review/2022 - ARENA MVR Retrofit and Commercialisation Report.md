https://arena.gov.au/assets/2022/11/mvr-retrofit-commercialisation-study.pdf

## Contribution

Looks at the cost of replacing the evaporators at the Wagerup facility in a retrofit, greenfield, and brownfield scenario. Wagerup is a lower temperature alumina refinery.

The MVR unit will take lower pressure steam from the evaporation stage, and compressing the steam to medium pressure steam ($60\times$ pressure). The electricity required for compression is supplied by renewable energy.
- This removes the opportunity present for power co-generation from boiler steam from the evaporation process.
## Content

Estimates that displacement of fossil fuels used in the Bayer process will reduce emissions by approximately 10MT CO2-e per annum. 
- Estimates that $4.5B and 1.2 GW of firmed renewable energy will be required to implement MVR across 7.4 Mtpa of high-temperature and 13.8 Mtpa of low temperature aluminium production capacity.

The MVR will enable additional capacity to drive a 65 tph single stage Falling Film Evaporator (FFE) responsible for the evaporation $Al(OH)_3$ solution that comes out of the digester after clarification.

- Design and operating cost is lower than conventional technology
- CAPEX of $220-$260/annual tonne for a greenfield project
- For a brownfield project, sunk cost of existing process heat and integration with existing equipment must be considered.

MVR also significantly reduces the water consumption of the evaporation process as it reuses the vapour from evaporation process that would normally be wasted.
### Australian Aluminium Processing

![[Screenshot 2026-07-30 at 3.56.39 pm.png]]

Upstream fugitive emissions and mining activities accounts for $3\%$ of the emissions.
## Alternative technology

| Technology        | Pros                                                                                                                                                                    | Cons                                                                                                                                                                                                     |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Electric Boiler   | There are some facilities that use electric boilers when there are excess hydro-generation. However, this is opportunistic and require duplicated base load generation. | Requires 3 times the amount of power as MVR. 3x CAPEX for renewable energy infrastructure and transmission.                                                                                              |
| Green Hydrogen    | However, it can use intermittent, non firmed generation, and the buildout is not equivalently 4x cost.                                                                  | There will be no water savings benefit and require 4 times the power to produce the same amount of heat compared to MVR.                                                                                 |
| Solar Thermal     | Potential for peak power cost periods.                                                                                                                                  | If the only off-taker is the aluminium plant, then it has to be financed by the refinery at a high hurdle rate. It also has low penetration, providing only 40% of the heat for the production facility. |
| Geothermal        |                                                                                                                                                                         | High cost, technically limited.                                                                                                                                                                          |
| Energy from waste | Look at Kwinana waste to energy project.                                                                                                                                | Highly site specific                                                                                                                                                                                     |
| Biomass           |                                                                                                                                                                         | Not sustainable for the amount of biomass required to fuel aluminium production.                                                                                                                         |
## Wagerup case study

### System configuration

![[Screenshot 2026-07-31 at 3.30.07 pm.png]]

There are 4 MVR trains that are used to deliver steam to existing refinery processes. There is also an additional digestion train that affects steam consumption but does not provide any steam by itself. Waste water is flashed to produce the vapour required for the MVR trains.
- Normally the vapour from the flash tanks is condensed and sent to a cooling tank.
![[Screenshot 2026-07-31 at 3.52.40 pm.png|697]]
- The sum of the compressors exceeds steam consumption by $8\%$ to ensure that boilers are redundant. 
	- ~={red}The capacity of the MVR trains are at the limit of what's available in the market.=~ Since we cannot combine two smaller trains into one big train, there may need to be commercial development of larger MVR technology for commercial deployment. 
- The three existing boilers are decommissioned and put into long term hibernation to preserve integrity. 
	- This fixes issue of steam shortage when boilers are down for maintenance.
- Use a Gas Turbine and Heat Recovery Steam Generator (GT-HRSG) during peak demand and fired to avoid capacity charges on the grid (as MVR is supported by renewables). The ramp time is $30$ minutes.
	- At a minimum, this is operated 18 hours per year.
	- Sized to enable 35MW and 177 tph of steam production $\rightarrow$ this is equivalent to a 40MW load reduction in the MVR train
	- Additionally evaporation can be turned down to reduce steam load by $56 MW$. The total load reduction is $113 MW$, which is $60\%$ of the $213MW$ of the refinery based power.

The system pressure is 880kPaA, matching the existing live steam system.
#### Design of MVR

The MVR is connected in series (10 compressors in series per train). Having this many in series increases the probability of outage.
- Shaft seals replaced once every two years and bearings require replacement every 10 years.

![[Screenshot 2026-07-31 at 4.33.57 pm.png|555]]

~={red}Modelling is done for peak refinery capacity=~

The first 5 compressors are variable speed to ensure flexibility of the flow.
- When compressor speed decreases, the pressure in the flash tank increases, which reduces the amount of vapor entering the MVR. The cooling water becomes warmer and more cooling load is placed on the cooling tower.
- Flue gas in the calcination phase is very moist. By passing the flue gas through a scribber where cold water runs counter current to the stack gas, the cooling water gains mass and temperature. This condensate is flashed to provduce vapour for M
## Research Gap

Uses 2 compressors in series and needs to be scaled up to a large-scale demonstration project. The technology have not been proven to power a high temperature process
- High temperature process requires a 60:1 compression ratio
- There are practical limitations due to the need to tie into the existing infrastructure and technical uncertainty around high temperature application of MVR

There is only one small facility in China that is using MVR for its alumina refinery as of 2022.

In scale up project, additional waste heat can be gathered from the precipitation, calcination, and digestion process in both high temperature and low temperature refineries to 

## Further research

- ELYSIS - partnership with Rio Tinto to remove GHG from the traditional smelting process
- Eco source is a smelter grade alumina that is produced with no more than 0.6 tCO2-e per metric tonne of alumina, half of industry standard.

Sunk cost into electrification when we also have to look at the recycling rate of aluminium?

Alcoa is also looking into solar thermal substitute for Bayer's process!




https://www.sciencedirect.com/science/article/pii/S026387622600496X

## Contribution

Using process data from an industrial plant, this work present an energy, economic, and direct CO2 emissions assessment of the implementation of MVR for evaporation ONLY of the Bayer's process.

Also developed an ASPEN-PLUS model for looking at evaporation process in the Bayer's process

Simulation was does in an Aspen Plus simulator for a multi-flash evaporator, which is most popularly used in industry.
- The one used in this study has 5 flash stages

The results shown was a 17.4% reduction in steam consumption and a 15.22% decrease in CO2 emission. 
- Because only the evaporation section was decarbonised

The economics was proven over a 5 year horizon with a TAC of 11.48% lower than BAU.

## Content

### Importance of evaporation

Evaporation has a strong influence on liquor cycle, refinery productivity and operating cost, as its output is the caustic soda used for digestion.

In multi-flash stage evaporation, the variables are the 
- Number of flash stages
- Theoretical minimum of flash stages is limited by heat and mass transfer, thermal losses, pressure drops, and operational constraints.
- Fouling history, maintenance conditions, and remaining service lives of the heat exchangers
	- Fouling occurs at above $100\degree C$, where development of scales compromises thermal efficiency and increase energy consumption.

When we are implementing MVR into evaporation stage, there are several implementation strategies.
- parallel approach where compressors are connected to each flash tank
- series approach that uses the waste steam from the last head
- Hybrid of the two options above
- Backup option is to maintain the original condensing and cooling equipment in case MVR is not available. Minimal impact on energy efficiency and evaporator availability.

### Industrial dataset

There were three industrial data sets with distinct operating conditions. one case was established as the base case and the other two operation condition was used to verify robustness of the base case. 
- MVR is applied onto this base case 
	- Scenarios with and without MVR were evaluated based on TAC, and impact of CO2 emissions.

| Process Specification  | Values          |
| ---------------------- | --------------- |
| Liquor temperature     | $123 \degree C$ |
| Evaporation rate       | 33.0 tph        |
| Live Steam temperature | $140 \degree C$ |
| Live Steam Pressure    | 361 kPa         |
ASPEN-PLUS models the complex thermodynamics of aqueous electrolytic solutions such as the Bayer liquor. The operating conditions were obtained via secondary sources. This was missing
- inlet and outlet pressures in the flash trains
- heat transfer areas and transfer coefficients of the HTX (calculated using iterative approximations)

### MVR implementation

Implemented compressor to the first flash train. This steam was mechanically recompressed and sent to the final heat exchanger
- The first flash stage was chosen to minimize the required pressure lift to reduce power requirements and capital investments.

MVR uses commercially available centrifugal compressors capable of increasing vapor pressure by up to 45% per recompression stage.
- 2 compressors were used in series with an assumption of $12\degree C$ per stage.
- Assumed isentropic efficiency of $83\%$.
- With no upgrades to the heat exchangers, constrained by heat exchange capacity.

A two stage compression engine was used to avoid overloading a single stage compressor although it is theoretically possible.
- This also enhances operational flexibility during higher spent liquor flow rates and to mitigate potential compressure degradations caused by liquid carryover.
#### Costs

The main cost of implementation was compressor and the electric motor used to drive it. This was used as a basis for costing the auxillary equipment.
- $\pm 50\%$ estimate.
- OPEX is limited to the consumption of direct energy sources
- Ignored the CO2 emissions associated with the electricity consumption of MVR compressors

#### Environmental


#### Operational differences

Reduced live steam consumption as the heat duty of the HTX connected to the MVR system increased. This reduced heat transfer in the remaining exchangers, leading to a $1\degree C$ decrease in the outlet temperature.
- Reduction of 17.4% (2.67 tph) of live steam consumption in the evaporation process.
- It is theoretically possible 

## Alumina refinery related readings

The barrier to MVR implementation, which uses flash steam from the Bayer process is 
- Production rate, caustic soda consumption, and the refinery's water balance.
- Can be adjusted to 600-800 kPa and 175-230 $\degree C$. 
- Refinery wide thermal integration is complicated. 

There is another study looking at 
- Spent liquor evaporation using mechanical vapor recompression: a means of boosting evaporation capacity. This study looks at increasing the capacity of an evaporation train in an alumina refinery using MVR, increasing evaporation rate by 30tph in 2005.
- In 2012, The research and development of mechanical vapor recompression evaporation energy-saving system, developed monitoring system for MVR and confirmed economic feasibility in a 15 tph evaporator, replacing traditional boiler with a 310kW electric compressor.
- Mechanical vapour recompression applied to alumina spent liquor evaporation plants. In 2019, showed application of MVR to the evaporation process for an industrial expansion project, increasing evaporation rate from 150 tph to 180 tph.
- [[2024 - ARENA MVR Implementation into Wagerup Refinery - Close Out Report]]
- Pathways to net-zero alumina: integrating low-emission technologies and policy reform in Australia. 2026. Energy savings of 50% and reduce 70% of the refinery's carbon footprint, and reducing water consumption by 35%.

There are also work done for precipitation
- 2024. Integrating vapor compression heat pumps and mechanical vapor compression with the Bayer's process. Explores a HP used to recover heat from the precipitation cooling circuit, with a COP of 2.69, and the downstream MVR unit can operate at a more favorable temperature levels, achieving a total COP of 3.65, reducing thermal demand by 29%.

There is also work done on digestion
- Assessment of multi-stage mechanical vapor recompression process for decarbonizing steam generation in an alumina refinery. 2024. Reduction of thermal energy consumption and carbon footprint

There is also work done on calcination
- Techno-economic assessment of integrated steam cleaning and recovery from alumina calcination. 2026. 



Studies has been done on the 



## Further Readings 

 Environmental and economic optimization of the pressureswing distillation process for separation of azeotropic mixture of acetonitrile-water.
 - Uses MVR for distillation, showing reduction of CO2 emissions by 75.18%

 Impact of distillation column design on potential for the integration of mechanical vapor recompression.
 - Shows lower economic cost (70% reduction)

 Thermodynamic assessment of MVR implementation in multistage evaporation plants. 
 - Shows the resultant energy savings and technology feasibility.
 
Enhancing the energy efficiency of a black liquor evaporation plant by mechanical vapor recompression integration
- Pulp and paper industry

Novel mechanical vapor recompression assisted evaporation process for improving energy efficiency in pulp and paper factory.
- Pulp and paper industry

 Technoeconomic assessment for black liquor concentration system of chemical pulp integrating mechanical vapor recompression. 
 - Reduction of steam consumption by 48.2%
 - 21.0% reduction in total energy cost and a payback period of 2.72 years - provided that black liquor solid content remains below 37.5% after the MVR stage\
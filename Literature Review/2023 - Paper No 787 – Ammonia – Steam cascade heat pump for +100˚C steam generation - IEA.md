https://heatpumpingtechnologies.org/publications/paper-no-787-ammonia-steam-cascade-heat-pump-for-100%CB%9Ac-steam-generation-14th-iea-heat-pump-conference-chicago-usa/

Collaboration between GEA, ANEO, and EPCON.
## Product Description
### ~={green}TRL: -=~

Produced steam from the ammonia heat pump can then be compressed to $2$ bar at around $120 \degree C$ with 4 centrifugal fans in series.

| Operating Temperature | Inputs                                                               | Limitations | Benefits                                                                                         |
| --------------------- | -------------------------------------------------------------------- | ----------- | ------------------------------------------------------------------------------------------------ |
| $85-90 \degree C$     | Water as low as $20\degree C$ or exhaust air from the drying process |             | High efficiency and minimises cost. Achieving temperature lift of 100K with a heating COP of 3.1 |
Produced steam from the ammonia heat pump can then be compressed to $2$ bar at around $120 \degree C$ with 4 centrifugal fans in series.

Uses natural refrigerants ammonia and $CO_2$ to achieve higher efficiencies. Ammonia heat pumps are preferred within the food and processing industry.

## Problem

- Many process are designed for $5-10$ bar of steam at $150-180 \degree C$ even if the temperature needed for the process is much lower
- Process heating demand above $100\degree C$ have often been met through electric resistive heating or gas fired boilers.
- We must select a refrigerant that can operate at above $100\degree C$ or at the high temperature range.
	- Kigali agreement: 2016 UN agreed that refrigerants with high GWP should be banned
## Content

There is a hierarchy to heat decarbonisation solution suggested by the paper. This is also suggested in [[2021 - Electrification & Renewables to Displace Fossil Fuel Process Heating]]

1. Energy efficiency 
2. Heat recycling
3. On-site generated thermal
4. Electric boilers
5. Renewable fuels
6. Offsetting emissions

### Reviewed refrigerants

| Refrigerant    | Positive impact                                                                                                                                                                                                                               | Limitations                                                                                                                                                                                                         |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| R245           | Have been around for $20$ years                                                                                                                                                                                                               | High GWP of $1013$                                                                                                                                                                                                  |
| R1223zd(E)     | Low GWP $<5$ and has a safety category of $1$                                                                                                                                                                                                 | Releases PFA into the environment, or contains elements that breaks down into a PFA.                                                                                                                                |
| R601 (pentane) | Critical temperature of $196.6 \degree C$ and therefore is suitable for ultrahigh temperature applications. Super-critical temperature is the point at which a vapor will not condense back into a liquid regardless of increase in pressure. | Highly flammable and therefore has a low safety rating.                                                                                                                                                             |
|                | It is also a natural refrigerant and has higher efficiency compared to other F-gas refrigerant.                                                                                                                                               |                                                                                                                                                                                                                     |
| R718 (Water)   | Supercritical temperature of $373.9 \degree C$. Can deliver temperature of up to $200\degree C$                                                                                                                                               | Higher boiling point at atmospheric pressure of $100\degree C$. This means that the steam compressors will need to have a large volume flow and operate in a vacuum with steam in vapor phase below $100\degree C$. |
|                | Non flammable, non toxic                                                                                                                                                                                                                      |                                                                                                                                                                                                                     |
## Solution

The paper compares the efficiency pure steam compression, single stage ammonia heat pump + steam compression, and two stage ammonia heat pump + steam compression. Their function is to raise waste heat to $120\degree C$ steam.

The heat pump solution is installed into a pet food manufacturing process.

![[Screenshot 2026-07-29 160353.png]]

- Assume that evaporation temperature is $22\degree C$

| Technology                                           | Pro                                                                                  | Con                                                                                                                                                                                                                                                                           |
| ---------------------------------------------------- | ------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pure steam compression using centrifugal compressors | 80-85% isentropic efficiency (highest provided by the centrifugal turbo compressors) | Each steam compressor can give $9-10K$ temperature lift. There are models that double this but is not economical at smaller capacities. Therefore requires 11-12 MVR turbo compressors.                                                                                       |
| Single stage ammonia heat pump + steam compression   | 88% isentrophic efficiency                                                           | At an evaporation temperature of $22\degree C$, the condensation temperature cannot be taken above $80\degree C$, and this will give a steam evaporation temperature of $76\degree C$, therefore, we will need 5-6 compressors to take the steam to the required temperature. |
| Two-stage ammonia heat pumps                         |                                                                                      | It is possible to raise the suction temperature of the high stage ammonia compressor, so that it no longer operates at the limit of its application area, allow higher condensation temperature. The steam evaporation temperature was $90\degree C$ as a result.             |
## Heat pump solution

Note that the absorbed power of the low stage compressor heat pump reduces around 2% per degree higher suction temperature.

Requires 20kW of oil cooling to lubricate the compressors, a high oil temperature will reduce viscosity and increase wear and tear of the heat pump.
- There are different solutions for oil cooling which increases heat recovery, but increases in difficulty of operation.

Higher suction temperature temperature reduces the pressure ratio of the compressor.

It is important to select the correct heat exchangers, some factors to think about are
- Sufficient support to hold high pressure at the condensation temperature
- corrosion of the shell element

Further steam compression is done with MVR technology.
- Uses MVR compact fans that are vertically arranged to get a temperature increase of 10K per stage. This uses water steam as the refrigerant.
	- We need a high volumetric flow rate at low pressure applications
	- High superheated steam temperature during compression
- Water (150kg/h) is injected to cool the superheated water steam back towards the saturation line.

The system is 1880 kW and uses 150kg/h of water to produce steam, producing 2 ton/h of process steam

Heat pump COP of 3.1 is obtained.

Compared with electric boiler with 90% efficiency, supplied by fossil fuel electricity. Reduced energy usage from 10.4 GWh to 3.03 GWh

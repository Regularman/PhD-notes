https://arena.gov.au/assets/2026/08/TES-for-industrial-process-heat-A-practical-guide.pdf
## Content

The study highlights that connection of thermal energy storage extends beyond capex and opex constraints. There are additional integration metrics which needs to be considered.

#### Design of the TES Integration

- We also have to think about other technologies. For example, MVR cannot use TES because MVR requires a continuous throughput of steam and waste heat, and does not allow TES to shift the demand away.
- Availability of biogas or onsite waste gas, which could reduce business case for TES. However, cheap renewables and competing use for biogas 
- The load profile also matters. If the heating load does not vary significantly across the day or season, then the opportunity for TES is not as strong. (If there is a even heat load, then you will have to oversize the heater to allow for charging during normal operation.)
- Implementation of TES is also heavily influenced by the energy efficiency measures already implemented onsite. If there is the site is not energy efficient, then the TES will be oversized.
- Where the TES is placed (between the heater and the load or as a pre-heater to reduce gas consumption). Alternatively, ESS is between the renewable energy and electric heaters.
	- ESS have shorter durations, lower lifetime, degrades overtime and lower round trip efficiency. However, it has lower standing loss, faster response time and is independent on service temperature. 
	- The TES can be in parallel or in series with the other plant, and this depends on considerations with the legacy assets
- The TES has to be designed such that heat can be reliably supplied to  the factory. Therefore, legacy equipment may have to be retained to ensure reliability. If the TES is between the heater and the system, then there will be lower resilience of the system. 
	- In scope of considering legacy asset, we also have to ensure that the legacy asset does not drastically change end-use equipment
- Site area is important, and this is also dependent on legacy asset, whether the project is greenfield or brownfield.
- Waste heat availability is extremely important as it will affect the booster heater required and heat exchanger design.

#### Design of the TES itself

- Dependent on if the process is iso-thermal (causing phase change) or sensibly heated
- Heating Transfer Fluid chosen needs to match and be higher than the process temperature for efficient heat transfer. (HTF can be steam, thermal oil, air, water, liquid metals, molten salts). 
- Mass of the TES is inversely proportionally with $\Delta T$, therefore a low $\Delta T$ reduces the mass and footprint of the TES. However, a large $\Delta T$ is responsible for higher costs of insulation materials, heaters, and ducts. Furthermore, a large mass is equivalent to a lower energy utilisation efficiency.
- The TES also have to take into consideration the energy-temperature profile. For example, steam systems require most energy inputs during evaporation, while smaller energy are required for condensate heating, feed-water pre-heating and steam super heating.
- Modular TES can reduce project risk through gradual enabling of TES units. However, more modular units have more surface area and therefore higher standing heat loss.

#### Consideration of the electricity network

 - ~={green}Network reticulation voltage=~ affects capex. Low voltage means large numbers of large transformers, excessive footprints, and longer installations time. However, lower voltage systems are more scalable and modular compared to higher voltages
 - Greenfield sites can design for additional electricity infrastructure. However, brownfield sites often don't have sufficient electrical connection capacities and upgrades may trigger extended shutdowns
	 - Upgrading voltage transformers, increasing grid connection, reinforcing internal distribution networks and integrating into existing EMS and control systems.
- ~={green}Network utilisation=~ is a metric (43%) in 2024. A higher network utilisation can lead to fixed costs being spread over a broader base and reduce network charge for everyone.
- Low ~={green}renewable curtailment=~ and increased ~={green}renewable fractions=~ as TES can soak up renewables during grid constraints.
- ~={green}Market signals=~ are important. If there are no period of cheap electricity, then the OPEX will not work out for the business case.
#### When considering the LCOH

- TES CAPEX, 
- electrical and process integration charge
- charging electricity costs
- renewable supply assumptions
- heat losses
- utilisation, which will depend a lot on tariff design and market price shape, which causes the TES to be activated at different times. Note that project finance scales dramatically upwards when going towards 100% capacity factor for the plant (in displacing the gas boiler)
	- There needs to be network and retail tariff structures that recognise the ability of the industrial load flexibility to reduce network congestion and support more efficient utilisation of renewable energy.
- amount of fossil fuel displaced (% of fossil fuel displaced)

#### When consideration operation of TES

We can optimise for 
- Lowest LCOH
- Lowest grid emissions
- Lowest network demand
- Highest production reliability
- Maximum heat availability

Note that further qualifications is needed to understand the grid benefit of TES. Further, any consideration of grid benefit comes from the perspective of the end user. However for the DNSP, they are a major stakeholder in this electrification business, so more understanding of the metrics used to quantify benefits for DNSP is also needed.


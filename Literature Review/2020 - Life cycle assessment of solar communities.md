https://www.sciencedirect.com/science/article/pii/S0038092X20307027

## Contributions

Highlights that there are a lot of studies into the implementation of solar PV, heat pumps, and heat storage to advance the idea of a net zero energy neighbourhood. However, most of these studies do not account for the life cycle perspective. 

Compares two scenarios, one where heat pumps (decentralised) are used for heating, cooling, and hot water demand, and a second scenario where centralised district heating infrastructure is powered by solar thermal panels with borehole seasonal thermal storage. (In the second case, heat pumps are used primarily for cooling)

Uses the ILCD 2011 Midpoint Impact Assessment method to characterise performance indicators.

- Simulation of energy resource provided by EnergyPlus 
- Simulation of energy systems for heating, cooling, and domestic hot water are performed using TRNSYS
- Canadian Weather for Energy Calculations (CWEC) data files

Want to find out if the initial energy and resource use can be offset by the higher performance of the system during the operation phase.

## Content
![[Screenshot 2026-07-22 134217.png|508]]
64 ha neighbourhood in Calgary, consisting of mixed used residential units, commercial, and institutional buildings.
- Advanced high performance building envelope consisting of high insulation values for walls and roofs (equal to 7 and 10 (m2.°C/W), respectively), in addition to triple glazed, low-e argon fill windows, and airtight construction.
- ASHRAE 90.1 lighting power density and electrical loads are based on standards and guidelines for all the buildings’ case studies. 
- Energy systems for space heating and cooling have high efficiencies, 
- Building integrated PV (BIPV) systems are assumed to cover the complete south facing roof surface. The gable roof has a 45° tilt, to allow near optimal energy generation from the BIPV systems. A specific “saw-tooth” with a 45° tilt angle is used for larger buildings, with south-facing surfaces having building integrated PV.

In this case study, the paper splits the neighbourhood into 16 quadrants, with each quadrant having its heating demand fulfilled by solar thermal systems.

### TRNSYS

TRNSYS was used in combination with national weather data to simulate enegry output of PV and solar thermal system in 30 minute timesteps. Each district is modelled separately, with stratified thermal storage tanks.

In the district, the fluid flow is controlled proportionally based on a P controller set on the thermal loads. Temperature setpoints for the hot water is $55\degree$ C

### Life cycle tradeoff

The lifecycle tradeoff we have to think about is the
- construction and maintenance of the distribution pipelines
- auxillary utilities such as PV panels

This is done over a 30 year timeframe

![[Screenshot 2026-07-22 134829.png]]

Solar thermal panels are sized based on data from Drake Landing Solar Community, which is one of the most successful documented example of a solar thermal community.
- Panels fixed in place with alumina devices, weight estimated based on commercially available system

The study had to optimise the area ratio between solar thermal and PV, based on heat and electric load as well as climate.

Heat load determines the fluid flow which determines the volume. A previous study has already been done on the neighbourhood, estimating electricity consumption.

### Results

Ultimately showed that there were up to 50% of impact reduction across all midpoints considered from using the solar thermal compared to decentralised heat pump

- Although varying by building type, the energy consumption per building decreases due to the replacement of heat pumps with solar thermal heating (maintained at 55 degrees celsius)

Validation through comparison with data from Drake's landing, which ahs a similar set up and is close in location to this hypothetical community.
## Limitations

Does not perform any type of optimisation. It is purely attributional
- Does not show demand profile and how solar thermal is able to satisfy this
- Does not comment on the end of life of both systems
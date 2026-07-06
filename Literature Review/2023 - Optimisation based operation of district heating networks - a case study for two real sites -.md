https://www.mdpi.com/1996-1073/16/5/2120

https://greenenergylab.at/projects/hybrid-dh-demo/?lang=en

Also known as the Urban Living Lab, Urban living lab at Neusiedl, testing various business models in connection with wind energy for a hybrid district heating system.

- 1 MW-th fuel gas condensation heat pump, a 1 MW-th air heating heat pump, and an expansion of the buffer storage tank to 300$m^2$ and a battery storage (700kWh), and a direct line between the wind farm and the heat centre.

As a result, there was
- a 20% reduction in the number of wind turbine shutdowns
- 5% increase in the proportion of renewable energy in the energy mix
- 2% optimisation in the DH system to reduce losses

As part of the project, Energie Burgenland developed wind to heat models, and a business model for wind to hydrogen.
## Contribution

This paper investigate the effects of integration of intermittent wind energy via a direct cable (which reduces the grid usage fee) or a boiler powered by biomass. There are also 2x water to water heat pumps and 2x air to water heat pumps.

Ultimately analysis shows that a reduction in fossil fuel based energy can be achieved despite high energy prices in the winter.
- The project is done in Burgenland, Austria, which ahs an over supply of renewable due to wind surplus. The economic value of wind energy can be increased by integrating it into the heating sector.

Mixed Integer Linear Programming is used to model the two District Heating network under consideration. The paper is interested in the economic efficiencies of a power to heat system.
- Additionally, increased electricity and gas prices from 2022 (due to the Ukraine crisis) is also considered to account for sensitivities.

The study was inspired by the instability caused by the Russo-Ukraine war and covid 19. The 2-3x increase in electricity production price had lead on effects to heat production. Gas prices also increased by a factor of 7.5 from 2019, and 1.3 by biomass.
## Content

Sector coupling is an important concept in the European Green Deal. This is where power industry also helps with heat production to achieve efficiencies.

Note that there are already many existing research on combined heat and power systems. 

### DH 1 - Biomas burner

Located in Oberwart with a biomass plant which feeds a district heating network via a heat storage unit. The plant is extended by a boiler to the local public grid with additional grid feeds

- Electricity between 1st September 2029 to 31st August 2020 were applied using the individual day ahead electricity spot market price
	- tariff of 3.327 cents/kWh
		- 1.4 cents/kWh for grid usage fee
		- 0.07 cents for grid loss fee
		- 0.352 cents /kWh for green electricity
		- electricity duty of 1.5 centrs/kWh
- Efficiency of 91% was used.
- 500kW-th rated biomass plant (lower operating limit of 500kW and a maximum operating limit of 5.8MW)
- 350kW e-boiler that connects to the local grid
- Maximum increase in heat production was 4.5MW/h
- Energy prices of 2ct per kWh

The heating profile of the district heating plant has a maximum heat demand of 4761.59 kW with an average load of 1547.65 kW and a standard deviation of 891.02.

![[Screenshot 2026-07-06 155721.png]]

### DH 2: Wind integrated district heating network

The district heating network in Neusiedl is originally consisting of a Biomass Plant and a gas boiler, which both fed the DHN via a buffer. 
- Directly connected to the DHN via a local wind farm with 30MW peak power
- HP cascade consisting of 2x air to water and 2x water to water heat pumps, which feeds into a buffer (power comes from the wind park.)

A flue gas condenser was also added to the BMP

In the summer, they would turn the BMP off, and use ambient air to heat up a "cold" storage tank. This is then used for a water sourced heat pump that feeds directly into the hot storage tank. 

In the winter, the cold storage tank is supplied by the flue gas condensor of the BMP. Gas boiler is used as a backup system, predetermined by the operator.

![[Screenshot 2026-07-06 160222.png]]

- BMP had a power limit of 520kW to 2600kW. 
- The maximum change in power is 780kW
- biomass price is 4 cents / kWh
- Electricity prices from Jan 2019 to December 2019 from the day ahead market
- The gas boiler is 3.9MW with an efficiency of 93%. The gas price is assumed to be 15 cents/kWh
- The maximum capacity of the buffer is 300$m^2$
- Heat pumps have a maximum thermal power of 2MW-th 

The network has a max demand of 5290kW, with an average load of 1706.43kW and a standard deviation of 1091.61 kW.

### MILP

MILP was chosen and implemented with an object orientated approach in Pyomo. Another option might be the Oemof framework.
## Limitations

## Questions

## Further Readings

[7] Effects of the addition of storage to a biomass boiler and a PtH plant. Shows that district heating demand in various DHNs in France can be sufficiently provided with biomass plants in combination with HPs and storage solutions.

[8] 5th generation heating networks, bi-directional low temeprature networks

[9] Installation of thermal storage can reduce the operation cost by 20%

[13] is an MILP formulation for the optimal control of combined heat and power plants. Verified with data from two turbines.

[14] Design for a 5th generation DHN based on ILP. The approach was tested on 2 real german sites. The results showed a 56% in carbon emissions and a 42% cost reduction.

[15] A tool for topology analysis for the optimal network for a given district.

[16] Modelling and optimization of the thermo-economic model of a district heating system.

[17] Proposed a model of an integrated electricity and district heating system based on thermal inertia of the heat networking and buildings on the demand side.
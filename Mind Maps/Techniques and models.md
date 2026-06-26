- F-charts: used to characterize the long-term performance of solar heating system (errors of up to $15\%$ due to approximations). It also models the solar fraction of the heating system, which is the fraction of the heat demand that is taken up by solar energy.
- System Advisor Model (SAM): Open sourced simulation model used to simulate PV systems, solar thermal, to geo-thermal, biomass combustion, and marine and tidal systems.
- Polysun: allows you to model solar thermal, heat pumps, PVs, and combined systems.
- TRNSYS: Model energy systems and perform simulations for transient systems
- PVsyst: models PV systems
- T$*$Sol: Customisable solar thermal models
- INSEL: simulation, monitoring, and visualisation of energy systems. Customisable in C/C++ or FORTRAN.

## Modelling tools

- ~={red}Centre Denmark =~provides a Trusted Data sharing platform to access historical data with data lake setup for smart energy services, used for forecasting electricity prices and control of heat pumps.
## Australian market modelling
- EZview - Spot market pricing (FCAS and ancillary market included) Check out Watt Clarity article for example [https://wattclarity.com.au/articles/2026/06/06june-regulation-fcas-trend/?_gl=1*ujguto*_ga*MTUyMDYyOTAyMy4xNzgwNTI2NzEy*_ga_4ZTT9PF6TR*czE3ODA5NjA0NzUkbzIkZzAkdDE3ODA5NjA0NzUkajYwJGwwJGgw]

[[2019 - Business case for heat pumps and thermal storage to replace straw-boilers in Samso, Denmark]] 

- EnergyPLAN: Priority list simulation model based on minimising primary energy consumption and ensuring hourly balance between supply and demand within electricity, heating, cooling, transportation, and gases. Suitable for looking at entire energy ecosystems rather than a plant.
- EnergyPRO is used to discuss business economic feasibility of DH schemes, and its optimisation against markets. It simulates, as a priority-list, the dispatch of different generation.

https://www.sciencedirect.com/science/article/pii/S0360544219325708

- Mixed Integer Linear Programming: Useful for solving unit commitment problems due to its flexibility in addressing the tradeoffs between system accuracy and the robustness of the optimisation method

https://www.researchgate.net/publication/317004288_Business_Models_Using_the_Flexibility_of_Heat_Pumps_-_A_Discourse

- Business canvas - looks at the stakeholders, value proposition, skills required for different business cases 

https://www.mdpi.com/2673-4117/7/2/85

- Uses PV system for solar and f-chart for solar thermal to conduct multi-criteria economic simulation and real performance analysis (as well as 3E (energy-economic-environmental) analysis)
- The f-chart correlates dimensionless variables of the solar collector system to establish relationships between these variables and the average performance of the system. Maximum error of 5% shown.
- F charts tutorial:
Deepika, D.; Baig, M.; Reddy, A.R.; Maneaih, D. Utilization of f-Chart Method for Designing Solar Thermal Heating System. IOSR J. Mech. Civ. Eng 2016, 16, 23–28.

https://www.sciencedirect.com/science/article/pii/S2949790625001570

- Uses ecoinvent, a database for LCAs, and the ReCiPe method to assess the effectiveness of various R-strategies (reduce, reuse, remanufacturing, refurbishment, replacement) in exploring the potential of circular strategies

https://www.sciencedirect.com/science/article/pii/S1359431125002947

- Used monte-carlo method for sensitivity analysis, it then uses the standardised Regression Coefficient (SRC) to quantify the sensitivity of the results on the input parameter

https://orbit.dtu.dk/en/publications/heat-pumps-supplying-district-heating-and-ancillary-services-for-/

- Used Dymola and its TIL library to model heat pumps
- Modelica is an open source object orientated programming language for the thermodynamic modelling of refrigeration/heat pump cycles (TIL suite, ThermoCycle, Vaporcycle Library)
- Finite volume method and moving boundary model for modelling heat exchangers
- Modelling the compressor using a steady-state mass balance and a dynamic energy balance to account for the heat stored in the component material
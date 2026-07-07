chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://infoscience.epfl.ch/server/api/core/bitstreams/4cfa7087-c9fa-4613-bfda-0e02e5a38beb/content
## Contribution

Research on the value of an industrial energy eco-system, using waste heat from beer and whisky making (0.061 kWh/L and 2.2kWh/L at 95$\degree$ respectively)

- Achieved overall utility consumption reduction of 22-63%
- 25-90% reduction in emissions

This highlights the significant potential for cross sectoral heat integration between breweries, manufacturing industry (low grade heat of ~80$\degree$C)

There was also a carbon negative solution in which it was economically feasible to capture biogenic $CO_2$
## Content

Process of the beer process was simulated with DWSIM which is a chemical process simulator (free and open source), and process integration was performed with OSMOSE [8].

Representing demand at an hourly resolution lead to substantial computational burden. K-mean clustering algorithm was used to aggregate the demand profiles into 15 representative operating points distributed across the year. The clusters had a silhouette score of 0.73, showing good separation.

- Assumes constant energy requirements from the manufacturing industry throughout the year, which loses some level of operational complexities.
- Some heating and cooling demand is supplied for heat pumps operating at different temperature levels.
- 


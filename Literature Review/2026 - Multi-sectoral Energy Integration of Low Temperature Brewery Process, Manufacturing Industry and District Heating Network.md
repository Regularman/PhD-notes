chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://infoscience.epfl.ch/server/api/core/bitstreams/4cfa7087-c9fa-4613-bfda-0e02e5a38beb/content
## Contribution

Research on the value of an industrial energy eco-system, using waste heat from beer and whisky making (0.061 kWh/L and 2.2kWh/L at 95$\degree$ respectively)

- Achieved overall utility consumption reduction of 22-63%
- 25-90% reduction in emissions

This highlights the significant potential for cross sectoral heat integration between breweries, manufacturing industry (low grade heat of ~80$\degree$C)

There was also a carbon negative solution in which it was economically feasible to capture biogenic $CO_2$, which is released by as a by-product of the brewery
## Content

Process of the beer process was simulated with DWSIM which is a chemical process simulator (free and open source), and process integration was performed with OSMOSE [8].

Representing demand at an hourly resolution lead to substantial computational burden. K-mean clustering algorithm was used to aggregate the demand profiles into 15 representative operating points distributed across the year. The clusters had a silhouette score of 0.73, showing good separation.

- Assumes constant energy requirements from the manufacturing industry throughout the year, which loses some level of operational complexities.
- Some heating and cooling demand is supplied for heat pumps operating at different temperature levels.

The paper proposes that the waste heat from the brewery can connect directly to the manufacturing industry or to the district heating network.
- The author creates a utility super structure built around the brewery to capture by products such as dregs, sludge, and biogenic $CO_2$, which can all be converted into Synthetic natural gas.
- Furthermore, the brewery also creates anergy, which is low grade heat that cannot be used directly for district heating. This anergy can be used as a source of heat for the decentralised or centralised heat pump.

System configuration is optimised through OSMOSE, with technology selection being driven by the total cost (sum of annual investment and operating cost.
- Factors in electricity price, natural gas price, and carbon tax level
- Sensitivity analysis is then performed to look at the influence of these factors 

### Results

Results are evaluated based on reduction in energy usage (efficiency) and reduction in carbon emissions. In the base system, heating 
#### Config 1 (full integration) vs config 2 (no integration)

## Questions

## Limitations

## Further Reading
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
- Furthermore, the brewery also creates ~={red}anergy,=~ which is low grade heat that cannot be used directly for district heating. This anergy can be used as a source of heat for the decentralised or centralised heat pump.

System configuration is optimised through OSMOSE, with technology selection being driven by the total cost (sum of annual investment and operating cost.
- Factors in electricity price, natural gas price, and carbon tax level
- Sensitivity analysis is then performed to look at the influence of these factors 

### Results

Results are evaluated based on reduction in energy usage (efficiency) and reduction in carbon emissions. In the base system, heating requirements is met with natural gas, and the cooling requirement is met with cooling towers and refrigeration systems.
#### Config 1 (full integration) vs config 2 (no integration)

In the sensitivity analysis done, there were only two settings for carbon tax. Furthermore, self reliance is increased when the electricity price is higher. This reduces the self reliance of the system as electric utilities are able to redistribute energy to meet both heating and cooling demand.

Analyse within a lifecycle framework where sustainability is first considered for the planetary boundaries before the economics.

Fermentation accounts of 14,440 k-ton/year out of 14490 k-ton of $CO_2$ emission.

The solution did not fully optimise for the carbon emissions, most likely due to a lack of BTM asset options.
- There are also scenarios where emissions is lower in scenario 2 compared to scenario 1, when electricity price is higher than natural gas price and carbon tax is 80 euros/ton. This increases the amount of available waste heat (heat pumps are more expensive to operate) to the rest of the network as it is recycled internally. This increases the reliance of natural gas.
- There is also scenarios where there are net negative carbon emissions due to the capture of biogenic $CO_2$, and converting it into e-methane. And increasing carbon tax level increased carbon negative performance. However, this is based on a certain grid electricity emissions intensity, which changes between regions.
	- Methanation and electrolysis are exothermic,. and the resulting heat generation constrains the maximum $CO_2$ capture due to cooling capacity limits. ~={green}(Can you invest in more cooling capacity to maximise the capture of biogenic $CO_2$?)=~
## Questions

## Limitations

need to do analysis from a environemntal framework first (locating planetary boundaries...etc, before we lok )

## Further Reading
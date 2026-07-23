https://www.sciencedirect.com/science/article/pii/S1364032117314314
Cited by 338

## Contributions

Outlines the pathways of waste heat utilisation for data centers, outlining how it can be implemented as well as a back of the envelope LCA analysis on its integration to district heating. It is a good reference to consider the different levers when optimising waste heat from data centers, as it presents its own risks and opportunities.

There are many studies that looks at the economic potential of data center waste heat utilization, but barriers are in place which prevents implementation. With increasing energy demand of chips, it is more reasonable to look towards cooling requirements in data center power usage.

Ultimately found that emission reduction depends on the emission and technology mix that is used as a reference. As well as consequential vs attributional standpoint.
## Content

### Data center operation

Data center locations are chosen based on 4 factors 
- Proximity to data users
- Proximity to cheap renewable electricity
- Geopolitical stability
- Abundance of cheap renewable energy that is reliable
If data centers were to connect to district heating, an additional requirement will be
- Proximity to heat demands
#### Cooling

Server racks are set up in hot and cold aisles to prevent the mixing of hot and cold that creates energy efficiencies and thermodynamics complexities. Note that almost all waste heat in a data centre can be removed.

| Type of cooling     | Return Temperature                    | Positives                                                                                                                                                                                              | Negatives                                                                      |
| ------------------- | ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| Direct Air Cooling  | Return temperature of $25-30\degree$C | Much less energy intensive                                                                                                                                                                             | Cannot be used for more modern data centres or in hotter temperatures/seasons. |
| Chilled air cooling | Return temperature of $25-30\degree$C | Uses a chilled water supply to cool the recirculating air in the server room                                                                                                                           |                                                                                |
| Liquid cooling      | Return temperature of $50-60\degree$C | On the chip cooling allows for much better heat transfer. Captures waste heat much better. Liquid cooling reduces the need for chillers and compute rom air chillers. Also increases chip performance. |                                                                                |
#### How is waste heat collected in data center

Almost all electricity consumed is converted to heat in a DC, but in 2018, this heat is mostly not utilised, due to a lack of transparency in data center operation and inexperience of data center operators to the energy market.

In 2015, waste heat was 3.3% in Finland and 8% in Sweden district heating.

Temperature of water in circulating water can be set to $60\degree$C. Waste heat can be captured from the returning waste heat stream, or the chilled water supply where the temperature is only $10-20\degree$C. 
### Metrics used to quantify waste heat potential in data centers

Metrics needs to be 
- Intuitive
- Definitive and purposeful
- Measurable
- Scales to technology, economics, and environmental changes
- Precise
- Granular

The study makes recommendations for metrics to be used for data center to categorise them and identify waste heat potentials. Changes in metrics also allow us to measure improvements from energy efficiency implementations. 

| Metrics                               | Description                                                                                                                            |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| Power Usage Effectiveness             | Total energy/IT energy, which is the energy used to maintain server racks rather than cooling.                                         |
| Energy Reuse Effectiveness            | Total energy - reuse energy/IT energy                                                                                                  |
| Power Density Efficiency              | Takes into account improvements in IT and cooling systems. It reflects inefficiencies in air flow thermal management                   |
| Data Centrer Energy Productivity      | How much work does IT equipment actually in the DC                                                                                     |
| Network Power Usage Effectveness      | Power consumed by network equipment                                                                                                    |
| Fixed to Variable Energy Ratio        | Provides an understanding of change and determines energy use at the electrical input for any device or group of device in the DC      |
| Return temperature Index              | Evaluates cooling air bypassing rack equipment. Measure of the net recirculation of air                                                |
| Supply Heat Index                     | Measures the separation of the hot and cold air streams. Ratio of the hot and cold aisles                                              |
| Return Heat Index                     | Measures the ratio of the heat extracted by the cooling system compared to the heat at the rack exit to under heat transfer efficiency |
| system Power Usage Effectiveness      | Effectiveness of a specific Computing Unit (cooling power and power consumed by specific computing equipment)                          |
| Data Centre Workload Power Efficiency | The specific workload, running on a specific HPC system                                                                                |
| Performance Per Watt                  | Actual energy efficiency of a device and how it is used, allowing for a global evaluation                                              |
### Barriers to entry

| Barriers and Risk                                   | Mitigation                                                                                                                                                                                                                                                    |
| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Low temperature (low grade waste heat)              | 5GDHC                                                                                                                                                                                                                                                         |
| High capex investments                              | HAAS. What happens in co-located data centres where the space is rented and cost is not borne by the users?                                                                                                                                                   |
| Need for ancillary heat production                  | Heat storage                                                                                                                                                                                                                                                  |
| Differing financial outcomes of DC and DH operators | HAAS. There is also the lack of data and transparency.                                                                                                                                                                                                        |
| Cybersecurity                                       |                                                                                                                                                                                                                                                               |
| Optimisation of thermodynamics                      | Mixing cooling and heat sources complicates the heat transference and fluid mechanics. Applying closed system principles to open systems oversizes the cooling capacity. Furthermore, there are dynamic power allocation based on the usage of a data centre. |
| Thermal losses                                      | DC must be located close to DH and heat demand                                                                                                                                                                                                                |
The cost of entry is dependent on the marginal production unit. Therefore, most likely only feasible for plants with expensive fuel such as natural gas. 
- The study considers the the emission factor of biomass to be $0$, highlighting that carbon dioxide will be released through decomposition anyways,
### LCA

Consequential LCA (CLCA) shows what happens when consumption or production changes due to technology implementation. The emission factor for electricity is higher as the first plant to reach to the changes are those that have the highest marginal cost. As long as these plants are running enough, then CLCA gives you an estimate of the short term impact. If the portfolio remains constant over time, then CLCA also provides the right resource for future. 

Attribution LCA (ALCA) looks at total emissions of the activity over a certain time frame and does not consider changes in consumption.

Performs back of the envelope calculation for emission calculations, but only for the operational aspect? Therefore, not fully cradle to grave.

**Table is for DC heat utilised as DH**
*Note that the CLCA considers displacement of CHP as marginal production unit* 

| Factor                                                     | Consequential | Attributional | Reason for difference                                                                                                                                                                                                                     |
| ---------------------------------------------------------- | ------------- | ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Avoided CHP production                                     | -95           | -38           | There is higher avoided CHP production in the consequential case as we are assuming that CHP is only activated during low renewable high pricing events. Compared to attribution, where emission is just a weighted sum of technology mix |
| CO2 emissions from electricity usage in DC Cooling and HPs | 23            | 9             | Higher level of CO2 emissions from the consequential case due to CHP during high pricing event. Assuming that biomass duels CHP and the emission in 0.                                                                                    |
| Net DH emissions                                           | 102           | 194           | There is higher avoided CHP production in the consequential case as we are assuming that CHP is only activated during low renewable high pricing events. Compared to attribution, where emission is just a weighted sum of technology mix |
The study also highlights that the cost LCA is very dependent on fuel prices and electricity prices, which are volatile to global supply chains. It depends on electricity build out 

- Assumes investment cost of $500EUR/KW_{heat}$ 

Ultimately, the decarbonisation potential is very dependent on the energy mix used in district heating. In this case, the LCA study actually found that carbon emissions went up, but that was on the assumption that biomass emission is 0 over its lifecycle. However, the cost of operation will decrease due to the estimated payback time of 5 years vs 15 years of operation life.
- This supports the many literature and paper that shows economic benefit of waste heat integration

- However there have been studies showing a lack of concern of data centre operators with a sustainability and energy efficiency according to a Fujitsu report on ICT sustainability. [60]. There is also CAPEX constraints that leads to ICT manager installing inefficient, cheaper cooling system.
### Levers

#### Where to use waste heat

There are many different places to use waste heat. Most studies only look at the optimisation of technology for a use case, but not the optimisation of use case for a particular technology such as data centre,

Waste heat can be used for own consumption such as space heating, domestic heating, melting snow, producing cooling through absorption heat pumps.

While external uses are drying biomass, preheating water in power plants, district heating, water desalination, and electricity production (low conversion rate).

Currently, in European DH most are 3GDH operating at $70-120\degree C$. They also do not have dynamic heat pricing.
#### Tradeoffs

![[Screenshot 2026-07-23 at 2.32.49 pm.png|363]]

Pros and cons of selling DC waste heat to DH.

| Pros                                                                                                                              | Cons                                                                                          |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Revenue from selling waste heat to District heating companies.                                                                    | Increased electricity consumption due to the operation of the heat pumps                      |
| Increases base load heat generation, and can operate flexibly during maintenance.                                                 | It can lower utilisation of ancillary heat production units.                                  |
| Connecting to district heating reduces the temperature lift of heat pumps operating for district heating compared to ambient air. | Increasing condensing temperature when using DC waste heat in DH reduces heat pump efficiency |
One of the main concern is if data centres can displace peaking generation capacity (i.e. preventing new peaking plants from being built). Otherwise, data centres will just reduce utilisation of existing ancillary heat production plants.
- The cost of waste heat must also be cheaper than the next marginal unit of production.
- The greatest benefit comes from avoiding the building of new natural gas peaking production units.
- Waste heat recovery will have to answer to fluctuation in IT loads on the intraday and on the longer time frame. 

Furthermore, data centres also have the option to use direct air cooling during winter (when heat demand in districts is actually the highest). Without dynamic pricing, there is no incentive for DC to participate in selling waste heat using heat pump booster.
- What if we use direct heat exchangers using 5GDHC low temperature grids?

We might need a DH spot market with dynamic pricing to incentivise DC participation.

#### Legacy Data Centres

There are 4 options for data centres that have insufficient power and cooling capacity.
1. Modernise existing DC
2. Invest in a new DC
3. Migrate workload to a larger DC
The first three options gives you options to implement new waste heat recovery technologies.
4. Do nothing
## Limitations

## Further Readings

There are many case studies that already looks at waste heat utilisation. Look particularly in example of Apple in Vyborg, Denmark. These case studies provide examples of waste heat that is available at different sizes.

Yandex and Telia publishes Global Reporting Initiative to understand and communicate the critical impact of businesses on sustainability.

### Examples of DH and DC symbiosis
[63], 

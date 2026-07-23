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

| Barriers and Risk                                   | Mitigation                                     |
| --------------------------------------------------- | ---------------------------------------------- |
| Low temperature (low grade waste heat)              | 5GDHC                                          |
| High capex investments                              | HAAS                                           |
| Need for ancillary heat production                  | Heat storage                                   |
| Differing financial outcomes of DC and DH operators | HAAS                                           |
| Cybersecurity                                       |                                                |
| Optimisation of thermodynamics                      |                                                |
| Thermal losses                                      | DC must be located close to DH and heat demand |

### LCA

Consequential LCA (CLCA) shows what happens when consumption or production changes due to technology implementation. The emission factor for electricity is higher as the first plant to reach to the changes are those that have the highest marginal cost. As long as these plants are running enough, then CLCA gives you an estimate of the short term impact. If the portfolio remains constant over time, then CLCA also provides the right resource for future. 

Attribution LCA (ALCA) looks at total emissions of the activity over a certain time frame and does not consider changes in consumption.
### Levers

#### Where to use waste heat

There are many different places to use waste heat. Most studies only look at the optimisation of technology for a use case, but not the optimisation of use case for a particular technology such as data centre,

Waste heat can be used for own consumption such as space heating, domestic heating, melting snow, producing cooling through absorption heat pumps.

While external uses are drying biomass, preheating water in power plants, district heating, water desalination, and electricity production (low conversion rate).


## Further Readings

There are many case studies that already looks at waste heat utilisation

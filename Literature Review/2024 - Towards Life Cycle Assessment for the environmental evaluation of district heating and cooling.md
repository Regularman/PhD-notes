https://www.mdpi.com/2305-6703/4/3/7

## Contributions

Provides 66 case studies from 58 papers on the LCAs on District heating. The primary purpose of the paper is to outline the choices inherent in conducting LCA. The 5 aspects which are looked at are 
- Functional unit
- Database adopted
- Characterisation methodology
- Multifunctionality
- Modelling approach (attributional or consequential)

The study highlights that many papers that currently exists is confined to performing a carbon footprint analysis of the use phase. Therefore, this study only looks at papers with LCA. 

The study also converted the results of each study into $GWP/kWh_{th}$ to compare across the 66 case studies.

It should be noted that there are few literature that combines LCA with optimisation techniques.
## Content

### Functional Unit

Functional unit is chosen based on the goal and scope of the study. The authors highlight that functional were chosen based on if the LCA results were integral to subsequent district level considerations, or on optimization, or comparison of production facilities.

| Functional Unit                                     | Use cases                                                                                                                                            |
| --------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| Unit of energy generated                            | Used to focus on what is the carbon emission impact of produce that unit of energy, which is the functional requirement of district heating systems. |
| Unit of energy distributed                          | Used to focus on what is the carbon emission impact of produce that unit of energy, which is the functional requirement of district heating systems. |
| Unit of input energy to the generators              | Technical optimisation of the district heating system to maximise efficiency.                                                                        |
| Unit of input combustion material to the generators | Technical optimisation of the district heating system to maximise efficiency. Typically used for                                                     |
| No Functional Unit                                  | Focused on the amount of $CO_2$ saved without actually delving into the granular detail. Used in global on country level decarbonization strategy.   |
## Databases

Either used Eco-invent, GaBi or independent sources. Using different databases  can result in significantly different results, which makes data unreliable.

| Database                      | Descriptions                                                                                                                                                |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Eco-Invent                    | High geographic data coverage                                                                                                                               |
| GaBi                          | Used for specific                                                                                                                                           |
| Primary and secondary sources | Primary sources are measurements and collected data and company record. While secondary sources are general estimates, scientific literature, and dtaabses. |
### Characterisation method

Characterisation methods are published methodologies used to assess midpoint impacts from the industrial activities.

| Characterisation Method |                                                                                                                                                                      |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ReCiPe                  | Has the ability to provide comprehensive information and a balanced approach between detail and synthesis, even at a global scale, thanks to its proposed indicators |
| CML                     | Chosen for academic purposes and applications related to industrial research and development.                                                                        |
Note that there are only the 6 studies that looks at 5GDH.
## Scenarios

Scenarios are usually compared with the existing district heating system or the fossil fuel based system. Scenario comparison is not provided only when the paper serves to prove a more general concept.

## Attributional vs Consequential approach

Consequential approach is about how we can change the consumption system to change the environmental impact. It seeks to capture the change in material flow that occur as a consequence of adding or removing a specific human activity.

While the attributional approach describes environmental impact at a given point in time given a system. It seeks to assign the environmental impact of the specified human activity within a given material flow in a system.
- We want to monitor every step of the system and find the hotspot within the product life cycle.

There are significantly less consequential approaches in the assessed literature due to its complexity.

## Multifunctionality

When there are multiple products out of the system , such as electricity and heat out of a CHP plant, we have to allocate the emissions based on different strategies. Also relevant tot he production of steam, hot water, electricity ..etc. 

The choice of allocation affects the emission intensity factor.

| Allocation method                                    | Descriptions                                                                                                                                                                                                                                                                                                                                       |
| ---------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Substitution method (ISO14044)                       | The impact of the primary product is determined by the different between the emission factors associated with that specific product and the emissions factor associated with the marginal production of the by-product (the impact the by-product will incur on the external system if it were produced by an independent activity out of context) |
| Partition method (ISO14044)                          | Allocation factors come from economic or physical characteristics of the generation system. The allocation of the factors is heavily debated.                                                                                                                                                                                                      |
| Incremental Electricity-Centred Reference (Outdated) | Allocates emission factor of electricity as if there were a separate production system for it. It allocates the entire benefit of co-generation to heat production                                                                                                                                                                                 |
| Incremental Heat-Centred Reference (Outdated)        | Allocates emission factor of heat as if there were a separate production system for it. It allocates the entire benefit of co-generation to electricity production                                                                                                                                                                                 |
| Surplus method (ISO14044)                            | The impact is assigned entirely to the main product                                                                                                                                                                                                                                                                                                |
| Separate Production Reference                        | Relative proportion of emissions they would require in separate production facilities. However it has limited adaptability to local context and temporal fluctuations make it unreliable.                                                                                                                                                          |
| Self tuned average Local productions reference       | Similar to SPR, and the data should be location specific.                                                                                                                                                                                                                                                                                          |
| Exergy method                                        | Allocates co-generated electricity and heat based on the exergy associated with thermal and electricity production. But this requries detailed knowledge of complex thermodynamic process                                                                                                                                                          |
| Arbitrary 50/50 allocations                          |                                                                                                                                                                                                                                                                                                                                                    |
| Based on seling price                                | Tied to economics that is dependent on geographic factor and geopolitical fluctuations                                                                                                                                                                                                                                                             |

## Limitations

- In its definition of network typology, it highlights that 5GDHC is only low temperature and not bidirectional.
## Further Readings 

PV backed heat pumps
- [41], [45], [2], [49]
- [15] - Solar thermal

5GDH
- [44], [57]

Data centre
[55]

Carbon reduction over the whole life cycle 
[65], [67], [50]

Industrial ecology and how sustinable forest management can interplay with biomass heating
[66] 

[71] Climate profile of 4GDH in sweden


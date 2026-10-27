https://journals.aau.dk/index.php/sepm/article/view/11215/9024

## Contributions

Highlights the importance of geospatial information on the development of energy systems. In this study, they used 
- spatial variability of the heat demand
- total heat demand
- geothermal resource, waste to energy, and industry waste heat availability (available heat supply)
for residential space heating and hot water demand.

However, the objective metric was cost.

As a result, the study was able to prioritise regions in Europe which can convert to district heating in the most cost-effective manner. However, again, this methodology provides a basis for ranking rather than making an absolute assessment.
- This means that there is no decision boundary

Highlights that previous studies have primarily relied on simplified system modelling and does not model the spatial heterogenity of heat demands. 
## Content

The European district heating market only covers 13% of the heat demand share in Europe. Further, residential heat demand is $\frac{2}{3}$ of the total heat demand in Europe. However, this will be different in Australia due to different climate and consumption habits.

### Methodology

Heat atlas downscales national heat demand based on floor area data for residential and service sector buildings across Europe to a 1ha resolution
- It incorporates building age to make some generalization about the energy efficiency of the building
- Regions were aggregated to the NUTS 2 region, which has population between 800,000 and 3,000,000 inhabitants.
- Note that industrial land use was incorporated, but the load types were aggregated and not considered. Further, industries were only used as a source of excess heat

The potential of Waste to Energy (WtE) was identified through assume plant presence based on inhabitants. Cities with larger inhabitants ensure economic viability of WtE plants by providing sufficient heat and electricity demand.

Industrial sources were obtained from datasets from sEEnergies and aggregated the potentials of the plants within a $2km$ buffer around the $DH$ area.

Due to the 1ha resolution of the modelling, although the locations of wastewater treatment plants, metros, and supermarkets may change, their technical potential remains unchanged within the region.

Suitable regions for geothermal obtained from an existing dataset.
#### Thresholds implemented

Excluded grid cells with the $<400m^2$

Therefore, the methodology for choosing suitable areas depends on
- distribution grid cost below a national ceiling
- annual heating demand above a threshold

To reflect investment feasibility for geothermal, only systems exceeding minimum baseload capacities of $40$ or $70$MW were considered, as smaller systems are not techno-economically feasible.
#### Cost function

The cost was based on DH pipe costs, which were 
- linear cost ($c_1$) $664$EUR/$m$
- area-dependent cost ($c_2$) $2,610$EUR/$m^2$
### Results

Ultimately found that using thresholds of $50$EUR/MWh and annual heat demand of $1GWh$, ~64% of the heat demand can be met through district heating. However, $55\%$ is the most cost effective penetration, as it can be achieved at 50% of the total cost. 

Ultimately, to validate the heat demand accuracy and valid

## Limitations 

Does not the involve codesign with the power system

In this study, the evaluation metrics of heat demand and cost are inherently coupled, as the paper states that regions with higher heat demand will inherently by more cost-effective

Further, it is unclear if the modelling accounts for renewable penetration in the system. As the the discussion later highlights, the model does not capture peak load interactions or operational flexibility. **Therefore, the report implies the heuristic that district heating will increase  renewable penetration but does not go into the mechanism for how this can happen**
- This includes climate and seasonal demands
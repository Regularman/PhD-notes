https://onlinelibrary.wiley.com/doi/full/10.1111/j.1530-9290.2011.00375.x

## Contribution

Compares 10 environmental impact categories across three scales
- Micro (0.1MWe)
- Small (1 MWe)
- Medium (50 MWe)
For a CHP plant to be built in Norway. This means that we are looking at a centralised vs decentralised approach and the life cycle performance of each scale.

This is done in an attributional LCA format for CHP gasification with downdraft gasification for micro and medium systems and integrated gasification combined cycle technology for the medium scale.
## Content

Functional unit = 1MJ of electricity and 1MJ of district heating delivered to the end user.
Uses the CML 2 Baseline 2000 Impact assessment, chosen for its holistic set of impact categories.

The main levers at the three different scales are
- grid and district heating losses
- Biomass procurement distance
- CHP plant emissions
- average electricity and district heating distribution distance
- Overall thermal and electrical efficiency
![[Screenshot 2026-07-24 122634.png|206]]

Uses the Ecoinvent database for the majority of the foreground processes. 
- Assume that all fossil fuel and electricity and biomass is sourced locally.
- Assumes that a Scandavanian softwood forestry process was assumed

### Transportation process 

Biomass forwarding carried out with a 3.5-6 tonne lorry, with operational emissions adjusted to Norwegian standard.

For forest residual
- Medium = 115km
- small = 39km 
- Micro = 29km

For sawdust residual
- Medium = 110km
- small = 15km 
- Micro = 15km

This is based upon actual road distance from the sawmill to the city of Trondheim, where the medium CHP is assumed to be located.

![[Screenshot 2026-07-24 123454.png]]

- Therefore, one limitation is that these distances are pre-set rather than optimised through an algorithm
### CHP plants

Uses technical data from BioSynergi Proces ApS for information about downdraft gasification. This uses an appropriately sized ICE for power production.

Emissions and operational data of CHP plants come from the GEMNIS database for the integrated gasification process.

Capacity factor of 0.51 was used. This is what makes the study attributional rather than consequential, as it does not consider the marginal production unit.

Used an economic scaling factor of 0.7. Capital was based on a small scale CHP plant

### Allocation problem

- Price allocation is region dependent
- Energy output allocation does not take into account the quality of the energy
- Therefore, exergy allocation was chosen for this study. The exergy based fraction of environmental impact attributed to electricity for micro, small, and medium was 0.78, 0.72, and 0.69.
### District Heating system

3 pipe sizes were used. Used $km/GWH-yr$ as a basis for the calculation of piping requirement. 
- $0.305km/GWH-yr$ for the Trondheim region and $0.299 km/GWh-yr$ across the Swedish system
- Assumed a certain distribution across these three pipes in each scale based on actual pipe distribution of Trondheim Energi.
- Network losses were 8.1% (medium), 7.0% (small), and 5.0%(micro)

### Electricity System

Assume that $100\%$ of energy production from the CHP is consumed or lost locally.

For medium, small, and micro-scale CHP, electricity lost through the electrical lines to the end user was then assumed to be 9.3%, 2.4%, and 0.68, which were calculated form the estimated line length, material, and cross section at each scale.
## Results
![[Screenshot 2026-07-24 132603.png]]

The small scale has the best GWP. However, smaller CHP plants also have lower pollution control.
- Ultimately found that the micro-scale plant created has the least i
Compared LCA with previous studies for validations. 
## Questions

### Limitations

Static size assumptions and comparison rather than heuristic optimisation.

## Further Readings
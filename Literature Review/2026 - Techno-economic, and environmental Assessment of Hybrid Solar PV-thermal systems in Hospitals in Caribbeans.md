https://www.mdpi.com/2673-4117/7/2/85
Cited by 2
## Contributions

Addresses the gap in literature in the integration of PV-solar thermal systems as a CHP option, as well as its interaction with hospital HVAC systems.
- Uses PV system for solar and f-chart for solar thermal to conduct multi-criteria economic simulation and real performance analysis (as well as 3E (energy-economic-environmental) analysis)

Integration of the two subsystems allows the author to investigate synergies between PV systems and solar thermal technologies.
## Content

Provides equations to size solar systems and includes all efficiency losses in the system. Including factors such as soiling losses and temperature losses, but does not state the source of these numbers for the solar thermal system.

Much of the f-chart comes from empirical assumption, and the paper does not justify how these numbers are obtained.

Assumes that the solar thermal system replaces a electric heater or LPG heater. The solar thermal system used is also a Vitosol 300 H30 model.

Quick note about inverter sizing, the inverter is only needed for DC to AC conversion. So if the system is not grid connected and completely behind the meter, then we do not need the inverter set up.  But you might need it for the appliances and demand anyways.

`In my current ESS setup, I want to consume as much PV power as it comes in immediately because I have insufficient storage for it. So I have 11.5 kW of PV, inverters that I limit to 8 kW output (10 kVA grid-interactive, feeds the whole house). I could use a bigger inverter to handle all of that PV in the middle of the day. But instead, it goes to battery. If the battery fills up, I lose the potential PV production (which drives me crazy). So in my case, there is a direct relationship with what I am trying to do.`

The primary constraints are the surface availability, and different areas on top of a hospital building was assessed for solar resource availability.

Note that ambient temperature is a huge factor in determining the energy required for the hot water demand despite constant mass flow.

## Research Gaps

This level of analysis can be extended to thermal storage and how that can play into ancillary services. Currently, storage is based on use only, and does not oversize thermal storage for additional ancillary services.

Ultimately did not discuss the efficiencies between PV and solar thermal systems.

Plenty of economic simulation has been done for solar thermal systems already
- Lack of examples comes from industry (Small-medium industries)
Also does not consider the need for firming given hospitals being a high priority demand customer and a critical service.

## Questions

Wouldn't you have to include the carbon emissions created by the demand of installing the solar thermal and PV system? 
- The paper does include this at the end with specific values for the PV and thermal systems, however, these can be quantified with an initial payback period.
## Further Readings

[13] PV-T coupled to a heat pump
[27] PV-T integration for sustainable buildings in Pennsylvania
[52] Thermal comfort in hospital buildings, a literature review
[45] Utilization of f-charts for designing solar thermal systems
[24] Using deep learning for hybrid optimisation



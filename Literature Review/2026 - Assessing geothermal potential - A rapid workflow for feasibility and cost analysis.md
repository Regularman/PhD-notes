https://pangea.stanford.edu/ERE/pdf/IGAstandard/SGW/2026/Pettitt.pdf

## Contributions

The study modelled the hydraulic fracturing of intact rocks for Enhanced Geothermal Systems (EGS) and compared them against naturally fractured rocks. These models (dynamic fracture models are used to understand the permeability field of the fracture.)

Fracturing rocks increases permeability and thermal output of the reservoir. Therefore, the cost of energy in geothermal resources is highly dependent on subsurface conditions. However, there are also other factors
- Production wells must be positioned above the stimulated injector to exploit the vertical growth of hydraulic fracturers
- Existing natural fractures enhance thermal output (both in terms of decline of thermal output and thermal power)
- Well separation has a significant impact on thermal output with respect to hydraulic fracture length distribution. Additionaly, the density of clusters (cluster spacing) controlled the residence time and fluid flow through the fractures to optimise heat extraction and minimise heat depletion
- Zonal isolation (flow conformance) improves thermal output 

You need permeable flow for geothermal systems. Further, low flow rates of water in the passage is required for higher residence time and more heat extraction
- Stress permeability is dynamically computed during the Dynamic fracture model. THe model splits up the discrete fracture into geomodel grid
- The directional hydraulic conductivity tensor, fracture kinematics porosity, and other heat transport properties.
- Essentially, hydraulic fracturing is required to increase the surface area for thermal convection coupled with a relatively low flow rate within the stimulated volume to sustain viable thermal output

Also compared using vertical injectors and lateral doublets as geothermal extraction pipes, as well as open hole and closed hole designs![[Screenshot 2026-11-26 135103.png]]

# Results

Further, the composition of the underlying geology is also important. the paper highlights that the maximum drawdown ($75\frac{kg}{s}$) changes depending on matrix permeability and porosity difference between granite and a mix of sandstone and carbonate lithology.

Simulations showed that flow rates at a few specific perforations can dominate flow and quickly short circuit potential flow paths leading to non-uniform flow along the injector and rapid thermal breakthroughs. Zonal isolations is implemented by shutting off flows from perforations to equalize flow along the well bore and ensure more distributed flow, higher residence time, greater heat production, and to delay thermal breakthrough.
- Thermal breakthrough is caused by premature drop in fluid temperature at a production well caused by the injected liquid taking shorter, preferred path within the reservoir without absorbing enough heat from the surrounding rocks,
https://onlinelibrary.wiley.com/doi/epdf/10.1002/cite.70062?getft_integrator=scopus&src=getftr&utm_source=scopus

## Contribution


Ultimately, this study shows that the design of the MVR system can dramatically change the required compressor size and system retrofit required. Using water as a refrigerant allows for integration with the existing steam 
## Content

Electric boiler scenario will result in extreme increases in the electricity demand, which will lead to high investment cost for infrastructure.

However, what is the difference in using heat pumps vs MVR, is it the temperature that can be reached?

Especially MVR needs to scrub the waste steam from digestion and calcination due to the presence of mud in the vapor mixture.
- MVR also needs an additional boiler for start up (to produce enough steam in the condenser) as well as another condenser
	- Alternatively, you don't need the startup boiler in brownfield environments by maintaining the existing gas boilers to the steam grid for startups
- For heat pumps the specific vapor volume and evaporation enthalpy at the respective operation temperature and pressure are typical properties to determine suitability.
- Heat pumps have a lower footprint with the correct refrigerant selection

However, note that heat pumps also need a second reboiler for startup, and there is additional heat transfer resistance in the condenser, which means that the compressor need to compensate at a higher temperature differential, leading to higher inefficiencies.

## Water heat pumps

The volume flow on the condenser side in vacuum operation  can be high resulting in a large condenser and compressor. also, when the steam pressure is <6 bar, the material and design of the top condenser as well as the conditioning of the feedwater needs to be paid special attention.
- Low dissolved oxygen and pH value can corrode the condenser and cause leakage

## Revamping distillation column with MVR

Note that a reboiler is a heat exchanger that is attached to the bottom of an industrial distillation column that boils liquid to form vapor.

Need to consider the heat transfer area to see if the existing equipment is sufficient in providing the steam duty at a certain pressure. 
- In this instance, replacement of the bottom reboiler for the distillation column to account for vibrational issues caused by high volume vapor flow.

The natural gas boiler is required for startup and to provide additional heating duty to the column. However note that the other paper highlights that steam recovery is sufficient to provide all heating demand.

### Simulation

The paper simulates the MVR implementation for a stripping column and a process column.
- A compressor with a diameter of 1.34m compresses the vapor to 0.8 bar in two steps. The compressor has an electrical duty of 1.53MW. Since the head product (what's coming out of it) is toxic and flammable, compressor material and safety also needs to be controlled.
- We can reduce the volumetric flow rate through the compressor through evaporative water cooling, which split the waste vapor output between the heat exchanger and the bottom reboiler of the stripping column
	- This allows smaller piping to be used.
	- The second option uses 4 compression steams with an impeller size of 0.26m and an electric power consumption of 0.9MW

![[Screenshot 2026-08-06 103155.png]]


### Compressor type

You can also use a screw compressor to increase pressure ratio and reduce the investment cost by reducing the compression stage needed. However this would require the output to be de-superheated with condensate. There will also be high compression ratios.

Furthermore, the project shows that an additional 3.6tph of steam is still required from the grid to provide sufficient heating to the process column.
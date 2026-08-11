
https://arena.gov.au/assets/2024/07/Univeristy-of-Adelaide-Integrating-Concentrating-Solar-Thermal-Energy-into-the-Bayer-Alumina-Process-Final-report.pdf

## Contribution

Research by Adelaide University. Australian Solar Thermal Initiative. $87 million funding.

Looks at the application of commercially available molten salt storage, solar syngas, and production of high temperature hot air.
- thermal storage (7-14 hours) is required for the hybrid solar thermal system for net zero operation
- Hydrogen or biogas can also form alternatives for backup of thermal storage
- Quality is largely location dependent

## **Solar thermal systems -**
All large scale system configurations had positive internal rates of returns. The cost of CST continues to fall, which will improve the project dynamics.
- IRR = 6-13.5%
- LCOH = 22-30/GJ on average and 14-24/G on low estimates

### **Solar reformed syngas**

Storage of heat is better than storage of syngas.
- Also facilitates more stable operation of the reactor
PCM thermal storage are cost effective solutions at the temperatures required to drive a steam reformer.

### **Solar calcination**

LCOH of 15.6/GJ including cost of heat transport if 40% reduction in capex and 40% advances in efficiency is accounted for. Based on current numbers, the LCOH with air as a heat transfer media, for retrofit, is 37.4/GJ.
- However, when we use hot air as the working fluid, there are constraints and upper limit on the heat that can be transferred.
- Obvious scaling effect up to $450 MW_{th}$.

UA did work on modifying the operation of an alumina calciner so that it can operate in a steam rich environment. 
- Also found that the produced alumina is different when it is created in steam rich environment, such as higher surface area, slot shaped pores. Steam calcination can also be achieved at lower temperatures, offering potential for lower energy consumption of the calciner.
	- More work needs to be done to see how steam will influence the grade of alumina produced.

Potential to use MVR when we are using steam. However, the scrubbing process required for this has not been commercially demonstrated.

The technology used for solar calciners is made possible through Solar Expanding Vortex Receiver (takes return air from the plant and reheating it to temperatures above $1100 \degree C$) - TRL 3-4.
- Requires further cold flow experiments and numerical model to understand upscaling potentials in single phase and two-phase flows
- From experiments done to validate CFD calculations in particle egress, flow field measurements of velocity, and particle number density. This led to the development of an optimised solar expanding vortex receiver.
- Lab scale demonstration for high temperature air receiver (efficiencies of $80\%$). Uses particles to achieve high radiation adsorption through an open aperture to transfer heat to the air
- Technically limited by ingress of cold air and particle egress, which requires further research

Looks into three main technologies

- Reforming of methane or biogas through SMR
- CSP calcination, more specifically
	- Direct heating
	- Heating with hot air
- molten salt (sensible heat) TES

Looking at net zero implementation of these technologies.
## Content

### Molten salt TES and solar thermal steam

To reach solar shares of 29-45%, we need 7-14 hours of molten salt thermal storage. These systems are expensive.
- Could be backed by hydrogen or biogas

Extremely site dependent, there may be lower qualities around Perth. Costs are expected to fall with the falling prices of CST. 

IRR values of 2.5-7%. LCOH on average is estimated to be in the range of 22-30/GJ.

## Solar reform of syngas

Done through SMR, where heat is used to split natural gas into hydrogen and carbon monoxide.
- Facilitated by a catalyst (often nickel)
- Before hydrogen via adsorptive separation, we get syngas
- We can add steam (700-1000 $\degree C$) to the syngas and it will reach with the carbon monoxide to make more hydrogen
$$CH_4+2H_2O\rightarrow CO_2+4H_2$$
Even though we get $CO_2$ still, hydrogen is an essential material used in fertiliser, plastic manufacturing, and fuel refining. Furthermore, the use of CCS can reduce the carbon emissions of SMR by up to 95%.
- These SMR will be co-located with ammonia plant.
- A lot of traditional SMR reactors sell their excess steam to industrial customers in adjacent plants.
- Hydrogen for far-away customers are transported through liquefied hydrogen.
- Lifecycle of SMR hydrogen is normally accounted for using the GREET module

![[Screenshot 2026-08-07 at 9.22.17 pm.png]]

Hot syngas can be directly inserted into calciner to prevent the need for cooling the syngas before use.

It is most likely better to operate the syngas off sun due to the storage of heat being easier to manage and thermal storage enabling more the stable reactions.
- New thermal storage with solid particles was investigated for the application of solar calcination and syngas reformation
- Most likely will use biogas as a source of methane. However, this is most likely not feasible due to supply constraints.

Stored heat could be provided to a plant that costs around $15.6/GJ including the cost of transportation (in the scenario where 40% is taken off the CAPEX and the technology matures by 40%)

- Cost of heat integration has efficiency of scale up until $450 MW_{th}$, where it becomes $5\%$. 

## Solar thermal calcinatinon

If heat is used as a heat transfer medium, then the LCOH is $37.4/GJ.
- However, there are thermal constraints with using air as a heat transfer fluid, and upper limit of heat demand serviced is 50%.
- Alternatively, we can use steam for heating in calciners. Research shows calcination in steam creates a smelter grade alumina with higher surface area and slot shaped holes. It can also be done at a lower temperature, reducing the energy consumed.
	- More work needs to be done on how steam will affect phase change in the alumina
	- We can also recover the steam, achieving energy savings of around 20%. But we need commercially proven technology that can clean the steam.
	- Steam also has a higher radiation absorptivity.

## New Technology - SEVR

![[Screenshot 2026-08-08 at 10.36.36 am.png]]

AU developed a Solar Expanding Vortex Receiver for air heating. It reheats return air from 600$\degree C$ to above $1100\degree C$. This is in 2023, TRL 3-4. The developed scaled is $50-150 MW_{th}$. 
- single phase and two phase flow modelling conducted for up-scaling. By measuring flow field of velocities and particle number density and performance measurements of particle egress from the small scale receivers, we can validate CFD models. This is used for geometric optimisation for the design of the device
- Demonstrated at lab-scale that it can reach up to $1300\degree C$. Direct heat transfer to particles suspended in the solar receiver is the most efficient form of heat transport as it avoids the exergetic loss associated with heating a fluid through a tube
- Technically limited by particle egress and ingress of cold air. The study has limited particle egress, but commercial trial is needed to find the efficiency at scale
	- Developed an aerodynamic shield to prevent particle egress

The device is built with refractory lined steel.

There has been a preference for natural gas over coal due to lower risk for contamination of the end product with fly-ash.

Note that the device is only the receiver.
- There are solar concentration technology.
### How does the solution address existing problems

Currently there are no commercially available technology using concentrated solar thermal that can reach $1000\degree C$ .
- However, commercially available solar tower concentrators have been demonstrated to reach 1300

Technology on the market has difficulty reheating already hot air.

Previous experiments were only on windowed SEVR. Having an open aperture instead of a window makes the system more susceptible to wind and complex air flows.
- We need models for cross flows to make a stable reactor
- A buffer chamber needs to be added for control purposed to minimise particle egress and cold air inlet
Mass and energy transport of solids in a gas phase is also a new area of research.
The rate of production, reaction temperature, and product quality will be affected by different configurations of the CST plant.
- For example, hot air will displace some combustion gas and reduce pressure at which calcination occurs. (This can be fixed with steam, which has a higher partial pressure)

Currently, configurations can be beam up where the material gets transported to the top of the tower or beam down where the materials are at the bottom.
- Research and experiments are conducted to assess which option is better.
### Direct Heating

The alumina particles is transported to the solar tower for heating.
- Original concept ""Hydrogen production by steam-gasification of petroleum coke using concentrated solar power—II Reactor design, testing, and modeling."" - Z'Graggen from ETH Zurich
- Solid particle receiver also demonstrated in 2010. "Development and Evaluation of a Prototype Solid Particle Receiver: On-Sun Testing and Model Validation."
- Work is also done by the DLR, the German Aeronautical institute
### Indirect heating with hot air - SEVR 

## Experiments

Used Particle Image Velocimetry to measure particle and flow velocities within the device. This could be done since the device is made out of acrylic.
- Water is used as a working fluid under isothermal conditions, injected through a long pipe to get fully developed flow conditions. Water is seeded with hollow glass spheres with a mean of $10\micro m$ and a specific gravity of 1.05.
- Water discharged from the device was put back into a water tank

| Experiment aim                                                                                                                                                                                 | Diagram                                                                                                                                                                                                                                                                                                                                                                                                                                 | Results                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Particle Image Velocimetry to measure flow egress                                                                                                                                              | ![[Screenshot 2026-08-08 at 10.38.00 am.png\|259]]The velocity of the fluid flow is measured $1$ mm above and below the aperture.                                                                                                                                                                                                                                                                                                       | The device was able to produce a stable vortex with low or reversed flow near the aperture, showing that the flow can be controlled with the receiver length. Showed that in the device, the flow through the aperture is very low relative to the overall flow in the system. Also showed that system can accommodate a variety of solar resource over the course of the day.                                                                                                                                                                                                                                                                                                           |
| Suction system to minimise flow egress at different outlet and inlet velocity ratios. Velocity measured with PIV.                                                                              | Dimensions such as the chamber length-to-diameter ratios and conical expression angles are kept constant to provide complementary vortex velocity data to the last experiment. The aperture was also investigated under open or closed![[Screenshot 2026-08-08 at 11.21.55 am.png]]The secondary concentrator is removed in open aperture scenario and then tested with and without suction. Water was provided with two suction pumps. | ![[Screenshot 2026-08-08 at 11.29.44 am.png]]Flow is characterised by an internal circulating flow, creating a central recirculation zone, where the inlet creates a flow that propagates upwards near the edge. When the aperture is open, there is almost no flow through the outlet, but we can use suction on the outlet, with small flow ingress. Swirl strength is dependent on aperture size. When suction is used, the swirl strength decreases but without significant impact on the flow ingress and egress. Ultimately showed that flow ingress and flow egress can be independently controlled.                                                                              |
| Experimental study looks at outlet single phase gas temperature at the outlet vs air mass flow rates. Numerical study done to understand the temperature distribution and fluid concentration. | Used $1kW_{th}$ solar radiator. Heated air is measured at the outlet.![[Screenshot 2026-08-08 at 12.31.33 pm.png]]                                                                                                                                                                                                                                                                                                                      | Shows that air ingress and increased inlet air flow reduced the outlet temperature. Lower mass inlet flow rate also allows for more uniform mixing of the fluid inside the heating chamber, w more homogenous temperature distribution and concentration.                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Use laser induced fluorescence and phosphorescence to investigate 2 phase velocities for gas and particles. (Not in a solar thermal vessel)                                                    | The signals are separated from each other using optical filters. Uses $250 \micro m$ PMMA spherical particles suspended in a water cuvette. Phosphorescence tracers are placed in the liquid for measuring fluid velocity.                                                                                                                                                                                                              | Shows that this technique is sufficient to measure the movements of both the particles and fluid velocities                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Measurement of particle temperature and particle number density                                                                                                                                | Conducted under high flux radiation conditions for a particle laden jet, which is heated with a solid state solar thermal simulator (2.1 -35.5 $MW/m^2$). Uses phosphor thermometry and direct particle imaging to obtain measurements of particle temperature and number density under different fluxes.                                                                                                                               | Developed an analytical model of particle temperature, taking into account particle radiation absorption, particle re-radiation, convection between particle and gas, and particle sensible heat gain. The results showed that particle temperature values plateaus at approximately $150\degree C$ at heat flux of $20.6 MW/m^2$, rather than continuing to increase linearly as predicted by the analytics model. This may be due to convective cooling and radiative heat losses. Furthermore, also due to radiation induced buoyancy and turbulence generation on the particle fluid heat transfer which increases convective cooling.                                               |
|                                                                                                                                                                                                |                                                                                                                                                                                                                                                                                                                                                                                                                                         | Results also clearly shows proportional relationship between the particle number density and the particle temperatures.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Development of CFD and RANS (Navier Stokes) models. This is required to understand the heating and cooling mechanisms                                                                          | Looked at particle size and distribution as well as volumetric particle loading. Experiments and numerical studies done on particle statistics in 2-phase jets. Looking at the statistics of the rates of spread and decary of both particle velocity and concentration distribution.                                                                                                                                                   | Developed the RANS models, but need to assess the validity of the tool for the application of vortex particle receivers.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Lab scale demonstration under windless conditions using 1.1kW heat flux into 5kW the receiver                                                                                                  | Show that the windowless SEVR configuration is viable and provides performance data for the validation of CFD models. (Previous demonstrations were in thermo-chemical applications rather than air or particle heaters). The SEVR is complicated due to the non-linear relationship between the absorption of radiation with particle size, mass loading, imposed by the high centrifugal motion in the machine.                       | Found that the warm up time of the solar receiver is 1.5 hr. Also found that the total energy transmitted to the cavity walls through radiation and convection are reduced when increasing the particle loading. The lab scale receiver was able to achieve efficiencies of up to 70% and temperatures of $350\degree C$. Ultimately, the operation of the SEVR was successful.                                                                                                                                                                                                                                                                                                          |
| Develop CFD models of the receiver                                                                                                                                                             | Developed a single phase flow field with a 50MW industrial scale hybrid calciner                                                                                                                                                                                                                                                                                                                                                        | Sufficient agreement between experimental results and simulations has been shown. Note that the air is preheated to $600\degree C$ before being injected into the chamber and receives 50MW of concentrated incident radiation. Air is received at a rate of 30kg/s CFD results simulates for temperatures up to $860\degree C$ (Note that we need around $900\degree C$ for calcination in alumina processing) and finds that SEVR with an expander helps to achieve the higher required temperature by reducing ambient air ingress.                                                                                                                                                   |
| Investigation into impact of calcination technique on alumin grade                                                                                                                             | We want theta and gamma alumina (not alpha, which is the stable structure) for the Hall Hercoult process with the right moisture on ignition, loss on ignition, and SA requirements. It is already known that the effects of steam on Boehmite calcination is positive, but effects on gibbsite is yet to be understood. Note that combustion from syngas creates 30% higher steam concentrations compared to natural gas               | Found that dry conditions is the most suitable for the conversion of gibbsite into Boehmite. Under 80% steam conditions, the formation was limited to 6-8%. But at 50% steam conditions, gibbsite only required slightly longer times for calcinations. The presence of steam will inhibit the release of water molecule, thus requiring a higher temperature relative to what is needed for a lower concentration. There is some temperature at which the steam becomes a catalyst rather than an inhibitor. The yield of alumina from the bohemite/gibbsite is a function of temperature and time, and AU is investigating the optimal conversion time given different levels of steam |
|                                                                                                                                                                                                |                                                                                                                                                                                                                                                                                                                                                                                                                                         | However, steam has a positive effect on the SA. 80% steam produced alumina with almost 3 times the SA compared to SMA produced currently by Alcoa.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Techno-economic analysis of direct solar calcination at the Pinjarra and Learmouth site - through simulation                                                                                   | SEVR is used to provide hot air at $1100\degree C$ for indirect heating. This also allows particles with more desirable thermal properties to be used in the receiver, which has high solar absorptance and durability. Uses a Heliostat into a 50MW-th receiver. The aperture window is left open to optimisation.                                                                                                                     | For the beam up SEVR, obtained a maximum thermal efficiency of 74% in Learmouth and 70% in Pinjarra. Capital cost of the project will be around $42M, but this does not include balance of plant and storage costs. Another problem with CSP maybe the available footprint. This is an LCOH of 22AUD/GJ. Shows that the temperature can be achieved.                                                                                                                                                                                                                                                                                                                                     |
|                                                                                                                                                                                                |                                                                                                                                                                                                                                                                                                                                                                                                                                         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |

https://www.mdpi.com/1099-4300/28/6/693
## Contributions

Compares two types of district heating networks
- 5DGHC (aenergy networks)
- Hybrid SOFC-GT cogeneration units, with and without CO2 capture, which supplies electricity to network users, including decentralised heat pumps and optimising waste heat recovery

Ultimately shows that integration of SOFC (solid oxide fuel cell gas turbine) co-generation unit into the aenergy network allows for an increase in exergy efficiency increase from 13.6% to 21.3%.

To set the scene, global warming and heat island phenomena are reinforcing the
need for cooling even in the central to northern areas of the northern hemisphere, where
heating was the main concern until recently. The multiplication of data centers for AI
(Artificial Intelligence) with high cooling needs is a major challenge, but also represents
opportunities for waste heat recovery at the district level.
## Content 

To analyse the exergy efficiency, we can break the over all system into
- power plant
- district heating plant
- building plant
- room heat distributor

Tables for the exergy efficiencies of each subsystem was provided, along with the technologies to choose from. Extending on this, grid losses and network thermal losses can be implemented to further refine calculations of exergy efficiency.
- ~={green}This model can answer why low temperature radiators should be used and HTF should be distributed as close to the use temperature as possible=~

#### Difference between $4^{th}$ and $5^{th}$ generation networks 

4th gen district heating network operates at $65\degree C$ hot pipe and $45\degree C$ cold pipes or similar temperatures.

While $5^{th}$ generation heating networks can either be
- Two pipe bidirectional networks operating close to ground level temperatures, satisfying local eating through heat pumps and cooling directly or through local refrigeration unit. Water networks require large pipes and large pumping losses. While $CO_2$ networks uses the latent heat of vaporisation at high pressures (35-50bars). The use of latent, rather than sensible heat results in a higher heat capacity per unit of volume flow and requires the use of smaller pipe dimaeters
- There are also one pipe bidrectional networks that require on the energy balance between hot and cold users along the network.
#### Cogeneration with hybrid fuel cells (SOFC/GT)

Popular when both electricity and heat is required
- SOFC/GT have high electricity efficiency and low health emissions impacts
- They do not require expensive catalyst like those used for lower temperature proton exchange fuel cells
- Inputs of pre-reformed natural gas, biogas, or synthetic natural gas

SOFCs converts chemical energy from a fuel directly into electricity through an electrochemical reaction using a hard ceramic as an electrolyte
- Compressed air enters the SOFC cathode, while pre-reformed fuel (like natural gas or hydrogen) enters the anode. High operating temperatures (600°C to 1,000°C) allow oxygen ions to pass through a solid ceramic electrolyte, reacting with the fuel to generate direct electricity.
- The fuel cell have unexhausted anode tail gas that enters into a gas turbine combustion chamber to drive the generator.

In the anodic exhaust flow ($700-800\degree C$), there is $CO_2$, unexhausted fuel gas (mostly $H_2$). This is then expanded through an inverted Brayton cycle where hot exahust gas expands through a turbine to sub-atmospheric vacuum pressures before being cooled and recompressed back to ambient pressure.
- Steam condensation happens , and the compression only occurs to $CO_2$. The condensed water is separately pumped and less energy is needed to recompress steam
- The fuel is burned with pure oxygen to prevent $CO_2$ and $H_2O$ concentrations in the gas as high as possible.
#### Integration with $CO_2$ DHC

The anodic exhaust flow can be cooled at the same low temperature all year round with the DH stream to favor maximum steam condensation. This increases the electricity delivered by the GT and the dryness of the CO2 recovered.

The study considers two cases for the SOFC 
- A SOFC with reverse Brayton cycle
- A SOFC with reverse Brayton cycle and additional rankine cycle adding waste heat into the burner
In both case the gas turbine has a pressure coefficient of $3$.

Exergy efficiency can be calculated as $$\frac{E_{GT}+E_{SOFC}+E_{\gamma, CO_2}+E_{\gamma,water}+M_{CO_2}e_{d,CO_2}-E_{water-pump}}{E_{\gamma, comb}+\frac{M_{O_2}e_{d,oxygen-burner}}{\eta_{sep}}}$$
- Note that the mass flow rate of $CO_2$ from the system is negative!

The numerator is the electrical power obtained from the gas turbine and the SOFC, the remaining exergy transformation rate in the condensed water and $CO_2$, as well as the power required to operate the water pump.

$E_{\gamma, comb}$ is the exergy transformation rate of the oxidation network. $$E_{\gamma, comb}=\dot{M_F} \times EXV$$where $EXV$ is the exergy value of the fuel. Further, $e_{d,CO_2}$ and $e_{d,oxygen-burner}$ are the $CO_2$ and $O_2$ diffusion rates, Exergy diffusion represents the spreading of useful work potential as the system moves towards thermodynamic equilibrium through irreversible processes.

Note that we can calculate the molar fraction of $CO_2$ in the exhaust gas using this formula.

![[Screenshot 2026-09-24 at 1.53.32 pm.png]]
#### Integration of 5GDHC with SOFC

5GDHC has a cold stream for waste heat recovery and flue gas condensation, which improves $CO_2$ recovery efficiency
- The captured $CO_2$ can be re-entered into the district heating network 
- The $CO_2$ can also be stored to generate synthetic natural gas
- $CO_2$ can also be combined with a thermal-electric ESS (Carnot battery)

#### Evaluation of the district heating system

Traditionally, the energy needs of communities are reported in terms of heat rates. Energy and exergy composites allows us to account for the temperature required by the heat distribution system inside each building

![[Screenshot 2026-09-24 145150.png]]

 The main variable that is changed is the different levels of temperatures used for the heating network heat transfer fluid.
 - Note that exergy in a chemical fuel is higher than its energy, as the partial pressure of the exhaust gas can do work when it mixes with the environment
![[Screenshot 2026-09-24 at 11.21.39 pm.png]]

For 5GDH, the $CO_2$ DHC is the 
## Further Readings

Integrated optimization of adaptive CO2-based district and cooling networks into multi-energy systems.

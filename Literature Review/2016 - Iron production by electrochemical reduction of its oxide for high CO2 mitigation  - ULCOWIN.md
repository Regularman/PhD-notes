https://op.europa.eu/en/publication-detail/-/publication/4255cd56-9a96-11e6-9bca-01aa75ed71a1

## Contributions

Shows that high carbon value of 150euro/t-CO2 is required, as well as a price ration of electricity on coal of lower than $3$.

Provides a LCA and exergy analysis of the electrochemical process.
- Defines electrochemical mechanism - Particularly, the impurities of silica and alumina on the yield of produced iron is studied.

The goal of the study is to operate a laboratory pilot cell.
- Currently produced 3.6kg of iron from this process. Test trials have produced pure iron of $99wt\%$ purity with low overall Faradaic efficiency of 72%.

## Content
## Reference case - BF-BOF (with coke oven and sintering plants)

![[Screenshot 2026-09-10 141202.png]]

Note that this includes the electricity generated from COG and BF gas. This is pretty similar to POWER to STEEL example in terms of the numbers.
![[Screenshot 2026-09-10 142145.png]]
### Mechanism - Electrowinning

The electrowinning of iron (hematite) is based on the following reaction carried out in an alkaline aqueous solution (sodium hydroxide and water). The iron is reduced as a solid as ultra fine particles around 10 $\micro$m in diameter suspended in solution$$Fe_2O_3\rightarrow 2Fe +\frac{3}{2}O_2$$
The process occurs at $110\degree C$, the current density is $0.1A/cm^2$ at 1.7V. 
- Cathode - Graphite - Reduction - The iron is deposited on the cathode $$Fe_2O_3+3H_2O+6e^-\rightarrow2Fe+6OH^-$$
- Anode - Nickel - oxidation occurs that takes electrons to form oxygen gas which bubbles out of solution $$6OH^-\rightarrow\frac{3}{2}O_2+3H_2O+6e^-$$
Note that there is an impeller rotating the solution to agitate it and blend the liquid.

#### Reduction reaction

We need a voltage across the electrolyte to give the electrons enough energy to reduce, according to the reduction potential of steel. This has been mapped out in laboratory scale trials, as a function of hematite concentration and the voltage across the cell. The x axis is cell potential and the y axis is conductivity, which will increase as reduction capacity inceases.
![[Screenshot 2026-09-10 151203.png]]

- Convection has a lesser effect at high Fe2O3 content; the dependence of polarization curve on rotation speed is marginal.

Looking at the Faradaic efficiency, which is how well the current produces a certain chemical product. Note that there is a competing hydrogen evolution redox reaction with the water, which is shown at higher current densities. Found that the window for highest faradaic efficiency is 1-3 A/m^2, reaching 97% efficiency.
- ~={red}Is it possible to collect the hydrogen?=~

![[Screenshot 2026-09-10 151928.png]]

The iron ore can have impurities such as SiO2 and Al2O3 in it. The feasibility was established of electrowinning of iron from iron ores containing 10 wt% SiO2 and 0.5-1 wt% Al2O3 in alkaline solution without any further solution purification. Current efficiencies were typically > 85%. However, these may loosen the deposits and reduce yield of iron.

A good cathode is one that 
- Has good adherence to the deposit
- Mechanical strength to withstand fastening condition
- High overpotential for competing hydrogen evolution
- Material should be cheap and widely available
#### Oxidation reaction

Most energy loss take place in the anodic reaction of oxygen evolution, and lowering this over potential is one of the most important sources of energy improvement.

- The oxygen evolution reaction is a sluggish 4 electron transfer process and require an overvoltage to speed it up. minimising this overvoltage is required to reduce energy consumption in electrowinning.
- The suspension of hematite already act as a catalyst.
- Nickel cobalt alloy minimises this overvoltage optimally.
- Other solutions includes cobalt based oxide spinels in a nickel matrix to speed up the reaction.

Anode also needs to be designed for efficient transfer of electrons and capture of evolving oxygen gas.

### Scaling up the process - Development of a laboratory scale pilot

In the first pilot plant, low faradaic yield was reported due to electrolyte leakage, and the settling of the iron fines, creates short circuits that bypasses the redox reaction. The new pilot cell sets out to fix these issues to improve faradaic efficiency. Some other design changes made were
- Even current distribution on the cathode to control the growth of iron solid phase and uniformity of the reaction rate
- Tightening of the cell to prevent leakage of electrolyte and short circuiting. Previously, loosening of the cell was caused by the poor structural properties of the graphite cathode. This has been replaced with magnesium and cupronickel

The ULCOWIN cell version N°2 was operated eighteen times. Each experimental test lasts typically several tens of hours. It resulted in the production of weight significant iron samples. These experiments contributed to test if the technology developed checked the specifications.
- The electrocatalytic anode with nickel cobalt plating did not work due to the dissolution of cobalt during electrolysis at higher voltages. Remember that cobalt is plated on nickel to accelerate the 

During this second pilot trial, 3.605kg of iron deposit was collected with a 70% faradaic efficiency over the long term. However, short term efficiency was 91% (this was the maximum reduction rate shown in early lab scale trials), suggesting degradation of performance overtime. Some positives were 
- Showed that in situ harvesting of the deposit is possible on the magnesium and graphite cathode but not the cupronickel. Iron plates are harvested without dismantling the cells. Cupronickel is unsuited due to iron sticking and magnesium is hydrogen sensitive, fuses with hydrogen radicals in the iron to form magnesium oxide, which consumes the magnesium. Therefore, it is proposed graphite is used with stiff cupronickel support.

Based on the learnings of the second pilot scale tests, improvements have been made and CFD simulations 

### LCA

![[Screenshot 2026-09-10 141026.png]]

The LCA for electrowinning is high level and developed from the operational emissions perspective. 
- Note that the electricity for leaching uses a simple COP equation, $COP = \frac{T_{hot}}{T_{hot}-T_{cold}}$, which is $COP = \frac{1}{1-\frac{T_{cold}}{T_{hot}}}$. Hence, the electricity required is the $$heat \times COP$$However, I was able to calculate much lower electrical consumptions due to an error in the 


- The electrowinning step also assumes 95% Faradaic efficiency and 100% conversion on a cell voltage of 1.7V.
![[Screenshot 2026-09-10 at 11.11.39 pm.png]]

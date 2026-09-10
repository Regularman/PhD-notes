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

Looking at the Faradaic efficiency, which is how well the current produces a certain chemical product. Note that there is a competing hydrogen evolution redox reaction with the water, which is shown at higher current densities. Found that the window for highest faradaic efficiency is 1-3 A/m^2.
![[Screenshot 2026-09-10 151928.png]]

### LCA

![[Screenshot 2026-09-10 141026.png]]

https://iopscience.iop.org/article/10.1149/2.F06242IF/pdf

Electra does acidic electrowinning. The paper talks about how the process addresses the following three problems.

The pilot scale can produce $120kg$ of iron plating from iron ore that is too heavy in phosphorus for the BF and DRI process.
## Most iron ore exists as hematite (Fe2O3), which has kinetically slow dissolution in acid.

## Soluble iron has multiple oxidation states that are stable in aqueous solution (FeO4 2-, Fe3+, and Fe2+), whereas copper and zinc exist primarily as divalent cations.

This is addressed by separating out the electrodeposition process into two step
### Step one

The hematite slurry (primarily $Fe^{3+}$) is separated out through the reaction 
$$\begin{align}
Fe^{3+}+e^- \rightarrow Fe^{2+}&:E^0=0.77V\\
2H_2O\rightarrow O_2+4H^++4e^-&: E^0=1.23V
\end{align}$$
The charge is balanced as the protons generated in the anode moves into the acidified catholyte, which dissolves more iron ore, which consumes more acid and concentrates dissolved iron.

### Step Two

The $Fe^{2+}$ is split and fed into the catholyte and anolyte compartment of the cell. On the anode, the $Fe^{2+}$ is converted back into  $Fe^{3+}$ and returned to the acid regeneration block. While the $Fe^{2+}$ is reduced to iron metal $$\begin{align}
Fe^{2+}+2e^- \rightarrow Fe&:E^0=-0.44V\\
Fe^{2+} \rightarrow Fe^{3+}+e^-&:E^0=-0.77V
\end{align}$$
The charge is balanced by moving cations through a proton exchange membrane and anions through an anion exchange membrane. The electrolyte fed to the cathode is first treated for impurities in the ore that are dissolved to prevent affecting the iron plating process.

This keeps only $Fe^{2+}$ to be reduced at the cathode. The presence of $Fe^{3+}$ can discharge the plated iron and reduce the faradaic efficiency of the cell
## Unlike copper, iron and zinc are less noble than hydrogen evolution (HER) and, unlike zinc, iron has favorable kinetics for HER. As a result, copper and zinc EW technologies operate efficiently in highly acidic environments whereas high-efficiency iron EW requires lower acidity.

By moving the process to a two step process, the electrowinning process can operate at a much high pH compared to the acid producing OER in the first stage

Furthermore, another benefit is that electrodeposition is most effective at the 10-100mA/cm^2 range. Where as OER have been commercially demonstrated at 1000mA/cm^2. Thus, the first stage can rely on engineering design aspect typical of electrolyser and/or flow batteries to reduce capital costs by running at higher currents.

In both one stage and two stage approach, for every mole of iron plated, 0.75mole of $O_2$ must be evolved by OER.
- However in the two step process, we are adding kinetic overpotentials due to the additional reduction of $Fe^{3+}$ but these can be minimal. But because the first acid regeneration cell can be designed as zero gap, we're reducing the ohmic contribution of losses.

## Further works

- Lowering the OER overpotential for non-precious metal electrodes that are also stable in acidic and oxidizing environments.
- Robust, long-lasting, and selective separators. 
- Dendrite suppression and morphological control of metal electrodeposition reactions.
- Scaling systems to industrially relevant formats to make a true impact on industrial decarbonization
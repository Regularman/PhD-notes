https://arena.gov.au/assets/2025/05/Fortescue-Low-Temp-DER-for-Zero-Emissions-Iron-Core-Research-Interim-Report.pdf

Part of the ARENA Transforming Research Accelerating Commercialisation Research.
## Context

There are concerns with the scalability of electrowinning to produce millions of tonnes of ore per year.
- Beyond supply and demand imbalances, increased recycling will eventually lead to accumulation of impurities in scrap which will make it unsuitable for high-quality steel applications.

The baseline pathways for iron and steel making emissions are shown below, and is consistent with other references

![[Screenshot 2026-09-11 at 8.16.27 am.png]]
This is from IEA report from 2020 about achieving net zero.
- With DRI-H2, the total electricity required is around 4 to 5.5 MWh/t iron for the total H2-DRI process [2].
- Conversely, electrochemical process can achieve reduction through a theoretical 2.8MWh/t. This corroborates with earlier research, which states ~3.3MWh/t of hot rolled steel. [[2016 - Iron production by electrochemical reduction of its oxide for high CO2 mitigation  - ULCOWIN]]
- Furthermore, there is a less strict requirement for high grade ores with electrochemical processing

Iron mainly exports iron ore that is 56-62% iron.
- A significant increase in the demand for DR-grade iron ore is expected towards 2030, which currently makes up only 5% of the global seaborne market.
- There are pressures to decrease production for low grade iron ore, due to EAF production from China and increased high grade iron deposits found in Guinea
- Note that low grade iron ore can be converted into DRI ready iron through LEDER product.
## Mechanics

The full chemical reaction pathway for the electrochemical reduction of iron ore is shown below.
![[Screenshot 2026-09-11 at 8.37.12 am.png]]

Another advantage of the electrochemical pathway is that there are lower storage requirements and lower operation costs. Therefore the pathway to commercialisation will most likely be cheaper compared to green hydrogen reduction.

The cathode is a carbon fibres and a polymer matrix pressed onto a steel-backed plate. However, the carbon is delaminating from this plate during the electrochemical conversion of iron ore, leading to failure of the cell.
- This might be due to the reactivity between the polymer and the alkaline aqueous solution
- Or because the temperature of the cell is above the glass melting temperature which softens the polymer
- Currently finding suitable thermoplastics with glass melting temperature above $110\degree C$

The hydrogen gas produced can also adhere to the surface of the electrode, reducing the surface area in contact with the solution and blocking sites where the reduction of iron can occur. However, it is possible to suppress the Hydrogen Evolution Reaction (HER), by changing its onset potential.
- We can do this by changing the cell voltage so that the onset potential of hydrogen evolution is not approached.
![[Screenshot 2026-09-11 at 11.31.08 am.png]]
The first reaction is the reaction of free hydrogen ions in the electrochemical cell in an acidic solution. However, in a alkaline solution, the hydrogen must be disassociated from water, which carries a larger reduction potential. Therefore, there is significantly lower hydrogen evolution in alkaline solution.
- Hydrogen evolution can also be mitigated through the use of surfactant which repels hydrogen from the surface of the electrochemical cell. This discourages hydrogen evolution and also ensures that hydrogen bubbles do not stick to the cell, which increases turbulence and solution mixing to reduce the inhibiting impact of hydrogen evolution.

For corrosive resistant materials, due to elevated temperatures, common materials such as polyethylene, polyvinyl chloride, carbon steel cannot be used.
- Further, any oxidising agents present in the iron ore and the morphology of the iron ore also affect the metals.
- The polymers exposed to hot caustic may experience cracking due to sudden change in temperature, and potentially softening, degradation, or decomposition when exposed to caustic over a long period of time. 
- Similarly, the steels may corrode due to hot caustic, and there may be erosion-corrosion due to the abrasiveness of the iron ore. More importantly, catastrophic failure in the form of “caustic stress corrosion cracking” can happen with steels exposed to hot caustic. Hence, highly alloyed stainless steel like duplex, super duplex or even nickel alloys may be required.
Although, 316L and 2205 duplex stainless steel was used, there is a lack of data showing their operations in highly caustic solutions in elevated temperatures.

## Effect of gangue in the slurry

The dissolution of gangue in the slurry solution and its build up in the recycled electrolyte can inhibit the evolution of iron from the iron oxide ore.
- By testing iron oxide reduction in fresh caustic and saturated liquor, it was found that reduction occurred at a significantly higher level in fresh caustic. However, results varied widely between different batches of iron deposit. Inconsistencies also stem from inconsistent flow rate of slurries at different concentration levels
- Research is done to associate the flow rate with the iron deposit composition to enhance iron recovery.

### Effect of cell design on production of iron

- High degree of iron sticks to the stainless steel electrode. However, more tests need to be ran to determine if this process can be scaled up and what happens at longer durations.
- Furthermore, experiments showed that higher cell flow velocity (which impacts flow regime (the distribution of fluid phase across the cell), causes higher slurry iron concentration that is deposited)
- Cell stacking: 1 cell produced 19g of iron, 2 cells produced 31g of metal, and 3 cells produced 54g of metal.
### Ancillary services

This includes rectifier, electrolyte tanks, heaters, circulation pumps and gas vent system.
- This needs to supply the electrolyte at the correct composition, temperature, flow, and pressure
- Control the voltage across the electrolyser stack
- Gas control and return electrolyte

Note that iron fines is explosive when in contact with atmosphere, and the storage of these product will raise concerns with transport and storage.
- Can be addressed through briquetting for transport. Needs to exceed $5 t/m^3$ density can be achieved to prevent pyrolytic reactions
Since sodium damages the refractory lining of the EAF, the produced iron has to be rinsed thoroughly before insertion into EAF.
- Respond to this through the development of automated metal detection systems
- Silica and alumina are required to be below 3% for addition to an EAF or BOF. The DER product is currently meeting these levels, but if the feed ore is changed or the impurities are not appropriately managed this will need to be monitored.
- Nickel and chrome from the stainless steel has been detected in the iron product, which will have to be tracked.
### Next steps

Fortescue is developing a DER plant Pilbara operation to deploy the DER technology at scale. This plant will be known as the Pilbara Low Energy Direct Electrochemical Reduction Process plant (Pilbara LEDER Plant) hereafter. The Pilbara LEDER plant is targeted at a 150 tonne per annum scale.
- It should be noted that the confirmed LEDER specifications are anticipated to be finalised after the Financial Investment Decision on the process with the Fortescue Executive Board which (at the time of writing) is scheduled for March 2025

It is also recognised, that the pure green iron produced via DER lacks carbon. Hence, without carbon the melting point of the iron is significantly higher which may cause smelting operations to change (1536°C cf. 1147°C for iron with 4.3% carbon).
- They are investigating adding carbon to EAF to decreas
## Further Readings 

Fortescue has announced the development of a pilot plant at its Christmas Creek site to help derisk hydrogen-based reduction pathways and demonstrate the viability of using Pilbara ores as feedstock [4].

There is also a new Circored facility in Frankfurt opened by Metso

Boston Metal is the main player in the space of molten ore electrolysis, where the ore is electrolysis at $2000\degree C$ and has validated the technology at semi-industrial scale, currently working on the scaleup of their pilot facility in the USA [6]
- The major barrier is commercial viability of inert electrodes in a corrosive environment

ArcelorMittal and John Cockerill started the construction of the first low temperature, iron ore electrowinning plant in 2024 with operations are expected to start in 2027 [8]

Electra, a US startup founded in 2020, has developed a process dissolves iron ore in a water-based acid solution and uses electricity to electroplate iron.
- The company recently announced the commissioning of a small pilot facility in the USA and has ambitions to demonstrate the technology with a 50,000-ton plant before the end of the decade [7].
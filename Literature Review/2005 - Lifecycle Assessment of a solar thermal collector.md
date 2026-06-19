https://www.sciencedirect.com/science/article/pii/S0960148104003714

Lifecycle assessment is performed using international standard ISO14040. Analysis carried out on the basis of data collected in an Italian factory.
- Solar thermal plants is used for warm sanitary water demand in this case

Tries to show the lifecycle assessment of each component in a way that is as disaggregated as possible.

## Step 1: Determining the functional unit

1. Impact of the entire equipment: Presented as global quantities for the whole collector. There may be confusion as there are various typologies of collectors that can change the results
2. Impact per unit collector area: This does not reflect the economy of scales. Two collectors with the same total impacts could have different specific one.
3. Impact per unit of energy output. This is not suitable as the output is very location and weather dependent.

This study used option 1, which includes the 
- absorbing collector
- water tank
- external support
![[Screenshot 2026-06-18 at 2.56.17 pm.png]]

This study will define a dominance analysis of the main component of the plant.

## Step 2: Determining the impact of transport of materials

![[Screenshot 2026-06-18 at 3.04.15 pm.png]]

Once the material has been identified, the transport impact can be identified through energy and environmental impact associated with transporting 1000 kg of the material for 1km. 
- It was assumed that material was carried by trucks with 28,000 kg capacity
- A different assumption regards the glass transport, purchased from a foreign company, that is supposed transported by medium and high-capacity trucks. Having not further information, it has been supposed an averaged condition of half load transport for double way. 
- Specific impacts related to trucks have been referred to Italian studies performed by the Italian Agency for the Environment Protection

They considered mean distance values. But how did they calculate this mean distance value?

## Step 3: Considering the manufacturing process

![[Screenshot 2026-06-18 at 3.13.12 pm.png]]
This is the process flow diagram for the collector flow unit. Therefore, a process diagram has to be made for each of the component identified earlier.![[Screenshot 2026-06-18 at 3.15.23 pm.png]]
For each of the sub process, you have to understand the energy and material inputs and the material outputs (including waste)
- Dust approximated as 1.5% of process mass (according to Italian standard)

There are specific emissions for welding that is specified by standards. Although welding emissions depends on the electrode used, the use of standards enable an estimate. In this case Following the US welding classification, it has been assumed to use the welding rod class E6010. 
- Similar calculations have been done for dry plasma cutting. There was an assumption for the thickness of plasma cutting, assuming linear proportionality since standards is for a thinner plate.

## Step 4: Installations

Installation considers

- transportation from factories to retailer: functional unit of 1 tkm by a 28000 trucks, for 100km (both ways)
- transportation from retailer to user: functional unit of a van with 3500 kg with distance of 30km both ways
- installation impacts: fastening supports and water tanks

## Step 5: Maintenance

Assume a maintenance cycle of 4-5 years. This necessitates,
- travel of technicians (80km by diesel car)
- substitution of PVC gasket, sealing, magnesium anode, electrical resistors, thermal fluids 

However, the material and energy costs of increasing the demand of PVC gasket is not considered?

## Step 6: Disposal

This was done in 2005, when the solar thermal company has only been operating for several years. 

Disposal strategy is the transportation of the material to a landfill (occur by 28,000 kg truck, 50km both ways)

You also need to look at metrics around landfill management which the study has not done.

## Step 7: Overall energy analysis

This concerns with the energy flow throughout the life cycle of the product and can be split into
- direct energy: the energy used in the lifecycle step, including production, the fuel for transport. This includes the electricity used for production and installation, and the diesel oil used during transport.

	- This is be quantified as the end energy, which is the energy that is output for the user. However, we need to look at the primary energy, which is the energy required to deliver the end energy to the consumer, accounting for inefficiencies and losses.
	- A conversion factor for diesel, as an example, included all losses for extraction, refining and transport of diesel up to the filling station, or for electricity, the production and distribution of electricity.

- embodied energy: the embodied energy is the energy consumed by all processes associated with the production of the material employed in the functional unit's input. This relates to the heat of combustion of materials used as feedstock (not for energy). This is the calorific value of the material if they are burned after their useful life.
	- The embodied energy can be broken down into the fuel for making each component of the functional unit
	- The embodied energy in the feedstock (all calculated as primary energy). Italian database [26] is a starting point

From this energy analysis, the paper was able to find the split between the direct and indirect energy consumption. 
- Notably, the energy consumption for production is $<5$% of the **global energy consumption**.

![[Screenshot 2026-06-18 at 11.11.42 pm.png]]

From these energy analysis, the study is able to breakdown which process of the solar thermal collector requires improvement in terms of decarbonisation.
- For example, the substitution of thermal fluid represents a great amount of global energy consumptoion ($11.5$% of global)

![[Screenshot 2026-06-18 at 11.13.31 pm.png]]

## Step 7: Environmental impacts

The environmental impacts are

- resource consumption: 450kg of materials
- air emissions: 650kg of $CO_2$ emissions (dominated by indirect emissions $80-90$%)
- water emissions: Primarily from the indirect emissions
- wastes and solid pollutants

The environmental impacts can too be split into direct and indirect impacts.

- Direct impacts are those directly related to the production process
- Indirect impacts are those related to the production of inputs into the functional unit

![[Screenshot 2026-06-18 at 11.20.22 pm.png]]

These environmental impacts can be summarised into an eco-profile, looking at various environmental indices

- GWP global warming potential ($kg_{CO_2-eq}$ )
- Acidification potential
- Ozone depleting potential
- nitrification potential
- Photochemical ozone creation potential

We can then calculate the payback period for the solar thermal collector $$\frac{LCA_{energy}}{E_{useful}-E_{Use}}=\text{payback time}$$
Similar calculations can be down for the emission payback period

## Questions

1. How would you integrate circularity into energy analysis
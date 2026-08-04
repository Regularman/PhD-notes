chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://www.racefor2030.com.au/content/uploads/B3-OA-Project-Final-Report-July-2021-20210721a-compressed.pdf

## Introduction

In Australia, industry uses half of the total end use energy, out of which 37% is used in process heating, representing $750\frac{PJ}{year}$. 

- Fossil fuel accounts for 90% of this, which represents $675\frac{PJ}{year}$ 
- Natural gas is the most common fossil fuel, accounting for 57% of process heat requirement, which is equal to $427.5 \frac{PJ}{year}$. 

The report aims to support industry to decarbonise reliably and affordably, focused on processes that reaches up to $150\degree C$.  
- This represents $180 \frac{PJ}{year}$, 24% of all industrial heating requirements in Australia
- Process heat is provided continuously and at different rates via steam

Hierarchy of lowest to highest cost decarbonisation technologies
1. Renewable energy and energy efficiency such as solar heat pumps/MVR or electric boilers, solar thermal, biogas/biomass burning
2. Thermal Energy Storage
3. Green fuels, which includes biogas upgrade into biomethane, green diesel, and hydrogen

Looked at the consequence of uptake in BAU and accelerated scenarios. Through this, identified that there will be carbon and financial cost if the BAU scenario is realised. It is only through the accelerated scenario that we can achieve $600M$ in financial savings and $50\%$ reduction in carbon emissions by 2035.

![[Screenshot 2026-07-27 180142.png]]

## ~={orange}Alumina and non-ferrous metals=~

### Processes

**Energy for process heating:** Uses $176 \frac{PJ}{year}$ for process heating, mainly supplied by natural gas and coal
- 50% of heat is supplied at $< 250 \degree C$ and the rest at $>800\degree C$
- Circulating steam at $150-170 \degree C$ causes losses of $0.77 \frac{GJ}{t}$ and cooling water circuit in the calciner could lose energy by $0.35 \frac{GJ}{t}$.
**Carbon emissions:** $6$ aluminium refineries accounted for $2.8\%$ of Australian GHG emissions

| Process                    | Input                   | Temperature                                                             | Purpose                                                                                                                                                                                                                                                                             | Share of energy and GHG                                   |
| -------------------------- | ----------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| Refining (Bayer's process) | Bauxite                 | See below. Considerable heat is required for digestion and evaporation. | Refining low temperature bauxite into alumina ($Al_2O_3$)                                                                                                                                                                                                                           | $70\%$ emissions. Requires 11-12 GJ/t for heat production |
| Hall-Heroult process       | Alumina and electricity |                                                                         | Smelt alumina into aluminium. Alumina is placed into an electrolytic solution with a cathode and anode and is reduced to form molten aluminium at the bottom of the cell when electricity is placed into the process. Carbon combines with the oxygen to form $CO_2$ at the cathode | 14-15MWh/t for Hall                                       |
#### Bayer's Process

1. Preprocessing: Depending on the aluminium bearing mineral, there are different dehydration temperatures
	- Gibbsite starts dehydrating around $220-350\degree C$, bohemite ranges from $250-450\degree C$, and diaspore between $460-560 \degree C$

![[Screenshot 2026-07-28 102328.png|367]]

2. Bayer's process: 400kg of bauxite produces 1930kg of alumina, or 1000kg of molten aluminium (99.5-99.8% pure)
	1. Bauxite is hydrothermally digested with caustic soda, forming aluminium hydroxide, at $140-150 \degree C$ for gibbsite or $220-260 \degree C$ for bohemite and diasporite. The insoluble particles form a red mud. There is little chemical change, so all the heat in the steam is available as waste heat.
	2. Bauxite residue is separated from aluminium containing liquid through clarification at $100-105 \degree C$ 
	3. $Al(OH)_3$ is precipitated out of solution at $60-80 \degree C$. Evaporation occurs at $70-100\degree C$ 
	4. Calcination step is performed in rotary kilns or fluidised bed at high temperatures of $950-1100\degree C$. The water is recycled for leaching in digestion. Circulating fluidised bed reduced total energy consumption for calcination using efficient heat recovery. 
$$2Al(OH)_3+Heat\rightarrow Al_2O_3+3H_2O$$
![[Screenshot 2026-07-28 123744.png]]

Note that medium pressure steam at $170-200\degree C$ is used for digestion ($5.5-6 \frac{GJ}{t- output}$), evaporation $2.6-2.9 \frac{GJ}{t- output}$, precipitation $~0.2~ \frac{GJ}{t- output}$, and residual washing and storage of red mud $~0.7 \frac{GJ}{t- output}$. This steam usage is ~$50\%$ of the total energy consumption in the Bayer's process.
- Current steam is produced from natural gas or coal

#### Difference between low temperature and high temperature Bayer's process

In high temperature digestion ($270\degree C$), the bayer sludge liquid is flashed from $250\degree C$ down to around $70\degree C$. 
- High temperature Bayer's process is also required at a much higher pressure, $5 MPa$. Therefore, in a low temperature plant, the steam generated from natural gas boilers at a high pressure, can be passed through a co-generation/turbogenerator plant to sell electricity back to the grid. The steam is used at ~600kPa through the Bayer's process.
	- This cannot be done in high pressure plants due to high pressure requirements

In high temperature Bayer's process, the steam is injected directly into the digesters rather than through heat exchangers. Therefore, there is more evaporation that is needed in the evaporation stage. This is additional heat is provided midway down from the digestion flash train.
#### Waste heat

Waste heat is produced from
- Calcination ($120\degree C$ waste water and $150-170 \degree C$ exhaust gas)
- Precipitation
- Flash cooling of digestion residual from $180\degree C$ to $100-105\degree C$ for clarification

For example, Alcoa's Pinjarra refinery has half of its steam from the waste heat of its gas turbine.
### Technology advancements

| Technology                                      | Use case                                                                                                                                                                                                                                                  |
| ----------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Mechanical Vapor Recompression                  | Recycling of steam waste heat through heat exchange and recompression cycle.                                                                                                                                                                              |
| Heat pumps (electric compression or absorption) | Would be interesting to understand the difference between MVR and electric pumps (heat pumps are probably for lower temperature due to low COP with high temperature)                                                                                     |
| Fluidised gas bed                               | Replaces rotary kiln in calcination process for internal waste heat recovery. Also reduces energy usage per ton due to direct contact between the fluidized particles and the material. However, cannot be done for finer particles due to agglomeration. |
| Organic Rankine Cycle                           | Potential to turn heat into electricity for the Hall-Hercoult process?                                                                                                                                                                                    |
## ~={orange}Wood and wood processing =~

 Large biomass resources, 
 - 3% of world forests
 - 17% of Australian land area (concentrated on the East Coast)
 - 61% of log consumption is used for timber, wood veneer, and wood products manufacturer
### Processes

**Energy for process heating:** Uses $14.3 \frac{PJ}{year}$ for process heating, mainly supplied by natural gas and wood waste
- Drying of lumber is a bottle neck, as it is time consuming and expensive. Thermal energy for drying consumes up to $70\%$ of the total energy use for turning logs into value added products. 
- Currently steam is produced through natural gas or biomass (woodchips) ~$170 \degree C$
**Carbon emissions:** 

| Process             | Input                                                                                            | Temperature                                                                                               | Purpose                                                                                                        | Share of energy and GHG                                            |
| ------------------- | ------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| Timber Drying       | Sometimes air drying is used with the aid of minimal low-pressure steam. (Steam temperature of ) | up to $150 \degree C$. Air drying occurs at $20-38 \degree C$ and kiln drying occurs at $40-75 \degree C$ | Dried lumber should have $8-12 \%$ moisture. This is done inside a steam-heated, internal fan compartment kiln | $\approx 10\frac{PJ}{year}$ and $2-3 \frac{GJ}{t}$ of lumber input |
| Debarking           | Electricity                                                                                      |                                                                                                           |                                                                                                                |                                                                    |
| Sawing and trimming | Electricity                                                                                      |                                                                                                           |                                                                                                                |                                                                    |
#### Waste heat

Waste heat can be produced from
- Exhaust hot air from kiln drying ($35-55\degree C$)
- Condensed water from steam injection into the drying process

![[Screenshot 2026-07-28 123736.png]]
### Technology advancements

| Technology                   | Use case                                                                                                                                                                                                                                       |
| ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Vacuum kiln                  | conventional kilns loses energy up to 65% which can be reduced to 30% using vacuum kilns. These kilns are specialized drying chambers that lower atmospheric pressure to evaporate moisture from wood or materials at a much lower temperature |
| Air to air exchanger         | Recycles heat from the vented hot air from the drying process                                                                                                                                                                                  |
| Dehumidification of the kiln | Condensing water moisture on a cooling coil dehumidifies the kiln and increases evaporation and drying rate of the lumber                                                                                                                      |
| Wood waste gasification      | CHP production from wood waste                                                                                                                                                                                                                 |
| Heat pumps                   | Leverage waste heat from the drying process                                                                                                                                                                                                    |
## ~={orange}Pulp and paper industry=~

### Processes

**Energy for process heating:** Uses $21.2 \frac{PJ}{year}$ for process heating across 44 sites, mainly supplied by natural gas and wood waste
- $4$ million $m^3$ of wood log used for domestic pulp and paper. Which is an eighth of the wood supplied in Australia $32$ million $m^3$
- Paper making from pulp require s$4.5-6 \frac{GJ}{t}$ of dried paper, largely for drying 

**Carbon emissions:** 

| Process                      | Input                                                                   | Temperature | Purpose                                                                       | Share of energy and GHG                                                                    |
| ---------------------------- | ----------------------------------------------------------------------- | ----------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| Pulping (kraft process)      | The production of concentrated black liquor can be used to provide heat |             | Turns wood into an intermediate pulp. Produces a large amount of black liquor |                                                                                            |
| Pulping (mechanical process) | Electricity                                                             |             | Produces lower quality pulp used for newspapers and low cost products         |                                                                                            |
| Pulping (semi-chemical)      | Reduced thermal requirements compared to both process                   |             | Provides additional chemicals to the pulping process.                         | Introduces environmental complexities due to absence of chemical recovery in waste streams |
| Paper making -               | Mostly supply heat from natural gas                                     |             | Turning into thin sheets. This can be integrated with pulping or separate     |                                                                                            |

#### Kraft process (Chemical pulping)

- Pulp digestion ($65-175\degree C$) - MP Steam - $2.2-3 \frac{GJ}{t}$
- Pulp washing ($60-70 \degree C$)
- Pulp bleaching (if white product is desired) ($30-90 \degree C$) - LP Steam $2.3-3.2 \frac{GJ}{t}$
- Evaporation ($100-110\degree C$) - LP Steam $3-4.3 \frac{GJ}{t}$
- Pulp drying ($40-55\degree C$) - LP Steam $2.5-3.5 \frac{GJ}{t}$
- Lime kiln ($340-1200 \degree C$) - supplied by natural gas ($1.0-1.5 \frac{GJ}{t}$) in rotary kilns. This is important in regenerating quicklime from lime-mud to recycle chemicals used in the kraft pulping process

![[Screenshot 2026-07-28 131540.png]]

#### Waste heat

Waste heat can be recovered from
- Condensate in evaporator $50-60\degree C$
- Hot moist air from direct contact evaporator
- Waste water from digester and pulp washer
- Waste heat from lime kiln that runs at $340-1200 \degree C$
#### Paper making

- Stock preparation ($40-100 \degree C$) - LP Steam - $0.7-0.8 \frac{GJ}{t}$
- Drying ($70-90\degree C$) - LP Steam - $0.3-0.4 \frac{GJ}{t}$
- Press ($40-50\degree C$) - LP Steam - $2.8-3.8 \frac{GJ}{t}$

![[Screenshot 2026-07-28 134723.png]]
### Technology Advancements

Look at 

- `Energy efficinecy and GHG emissions: Prospective scenarios for the pulp and paper industry.`
- `Energy Reduction in the pulp and paper industry - an energy benchmarking perspective`
- `Pulp and paper industry: Energy Conservation`

| Technology                   | Use case                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Recovery boilers             | Instead of using conventional gas fired boilers to produce thermal energy, it uses black liquor, which is a byproduct of chemical pulp manufacturing, to produce thermal energy. Black liquor is sprayed into a combustion chamber. As the droplets fall down in the chamber, the black liquor goes from 18% solid to 68% solid using steam heat. The residual falls to the bottom (mostly carbon product known as green liquor). By adding lime to the green liquor, it turns back into white liquor used for digestion. Black liquor combustion can supply 80% of the heat demand, backed by natural gas. |
| Waste gasification           | Uses waste gasification cogeneration to supply the rest of the energy after recovery boiler. Look at Australian paper and SUEZ 600 million boiler.                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Heat recovery and waste heat | Reduce energy usage by $1.07 \frac{GJ}{t}$ of paper produced. ~={red}(World Energy Investment Outlook. 2014)=~                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
## ~={orange}Food Processing and beverage sector - Dairy Processing=~

Across the entire food and beverage sector, energy consumption for process heating was $119 \frac{PJ}{year}$.
### Processes

**Energy for process heating:** 
- Primarily uses natural gas for heating
- $0.53-1.5 \frac{GJ}{t}$ per $kL$ of raw milk is needed to make various dairy products. This causes 141 kg of $CO_2$ emissions
	- $8.3 \frac{GJ}{t}$ for milk powder, although 5.3 is the average for a modern factory
	- $1.3 \frac{GJ}{t}$ for cheese
	- $1.2 \frac{GJ}{t}$ for butter
	- $0.7 \frac{GJ}{t}$ for yogurt
	- $0.2 \frac{GJ}{t}$ for milk
- $84\%$ of energy is used for heating in dairy Australia
**Emissions:** 
- Dairy manufacturing has a lot of emissions from transportation.

| Process                                              | Input    | Temperature        | Purpose | Share of energy and GHG |
| ---------------------------------------------------- | -------- | ------------------ | ------- | ----------------------- |
| Pasteurisation                                       | MP Steam | $80-120 \degree C$ |         | $0.9-1.4 \frac{GJ}{t}$  |
| Pre-evaporation                                      |          | $65-75\degree C$   |         | $0.4-0.6 \frac{GJ}{t}$  |
| Spray drying and fluidised  bed dryers               |          | $35-200 \degree C$ |         | $3.7-5.8 \frac{GJ}{t}$  |
| Cleaning in place                                    |          | $60-65 \degree C$  |         | $0.3-0.5 \frac{GJ}{t}$  |
| Value adding process (Cheese, butter, yoghurt, milk) |          | $70-110\degree C$  |         |                         |
![[Screenshot 2026-07-28 140708.png]]

A note on spray drying, which is a method of forming powder form from a liquid. The milk is sprayed and atomised into a chamber where it is rapidly evaporated to leave behind the powdered product.
### Technology Advancement

- `Renewable energy options for Industrial Process Heat. 2019. ARENA`
- `National Pollutant Inventory` includes data on many food processing plants in Australia, but does not include smaller sites.
- `Eco-efficiency for dair processing industry. 2019 `

| Technology          | Use case                                                                                                           |
| ------------------- | ------------------------------------------------------------------------------------------------------------------ |
| MVR                 | Used in milk evaporation                                                                                           |
| Reverse Osmosis     | Used for concentration of the milk product rather than through conventional evaporation                            |
| Waste heat recovery | Rectification of steam leaks, using boiler condensate return heat, maintenance of steam traps, and pipe insulation |
## ~={orange}Food processing and beverage manufacturing - Meat Processing=~

Across the entire food and beverage sector, energy consumption for process heating was $119 \frac{PJ}{year}$. 
### Processes

**Energy for process heating:** Each typical red meat plant uses $3.3 \frac{GJ}{tHSCW}$. However, the exact consumption depends on the type of red meat being used.
- Primarily uses steam to provide the hot water ($82 \degree C$) or warm water ($43\degree C$) that is needed for cleaning and sterilisation. The boilers, supplemented by the heat exchangers with waste heat, uses natural gas or coal.
- Rendering is the most energy intensive process
- Freezing occurs at $-40\degree C$ and provides opportunities for waste heat recovery
- More than $65\%$ of electricity consumption comes from refrigeration to around $-40\degree C$.
- $7.9 \frac{kL}{tHSCW}$ required for the meat processing process, 30-40% of which is turned into hot water and warm water.
**Emissions:** 
- $432 \frac{kg CO_2}{tHSCW}$, which culminates to $1.3 \frac{MtCO_2}{year}$ for $3.1 Mt$ of production


| Process                             | Input       | Temperature        | Purpose                                                                                    | Share of energy and GHG |
| ----------------------------------- | ----------- | ------------------ | ------------------------------------------------------------------------------------------ | ----------------------- |
| Slaughter and evisceration          |             | $43-82\degree C$   | Separates into different components for processing                                         |                         |
| Hide processing                     |             | $43-82\degree C$   | Production of leather                                                                      |                         |
| Paunch processing and offal washing |             | $43-82\degree C$   | Edible offal and pet food production                                                       |                         |
| Blood processing                    | MP Steam    | $110-130\degree C$ | Blood producti production                                                                  | $0.9 \frac{GJ}{tHSCW}$  |
| Rendering                           | MP Steam    | $115-145\degree C$ | Done for 40-90 minutes per batch. Separate animal product into fat/oil, protein, and water | $1.7 \frac{GJ}{tHSCW}$  |
| Chilling                            | Electricity | $-4 \degree C$     |                                                                                            |                         |
#### Waste Heat

Waste heat can be recovered from
- Waste heat from the exhausted steam is recovered for generating the hot water and supply $60/70\%$ of the total energy needs for the plant's hot and warm water supply
### Technology Advancements

`Emission reduction pathways and opportunities for the Australian red mean processing sector. AMPC`

| Technology                     | Use case                                                                                                                                  |
| ------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Energy efficiency imporvements | $27\%$ energy usage reduction from $2008-2014$. Further suggests reducing the sterilisation temperature can reduce energy demand further. |
| Refrigeration heat recovery    | Taking waste heat from chiller condensers, which could provide supplementary heat from the boilers.                                       |
| Biomass boilers                | Look at AMPC report on emission reduction pathways and opportunities for the Australian red meat industry.                                |
### Case studies


### ~={orange}Food processing and beverage manufacturing - Beer Production=~

Across the entire food and beverage sector, energy consumption for process heating was $119 \frac{PJ}{year}$. 
### Processes

It should be noted that the addition of material is possible at various stage of the beer production process to give unique flavor profiles to different beers.
- Fermentation temperature are different based upon flavor profile. Temperature inversely proportional to fermentation time
- Low/no alcohol beer uses additional thermal separation process, or alternatively through reverse osmosis.

**Energy for process heating:**
- There is high variability in energy consumption for thermal energy ($43-226 \frac{MJ}{hl}$), typically between $83-144 \frac{MJ}{hl}$ for breweries that produce $10,000-1000,000 hl$ per year
- Low pressure steam is the main source of heating

**Emissions:** 

| Process                      | Input                         | Temperature       | Purpose                                                                                                                                                                                                                         | Share of energy and GHG                                                                                                              |
| ---------------------------- | ----------------------------- | ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| Grain mashing                | LP steam ($130-160\degree C$) | $45-75 \degree C$ | Crushed malted grains are mixed with hot water to activate natural enzyme, turning insoluble starch into simple fermentable sugars that goes into the wort solution. A mash/lauter tun is just a big tub that steeps the grain. | $4.9-8.5 MJ$                                                                                                                         |
| Hop/wort boiling             | LP steam ($130-160\degree C$) | $95-100\degree C$ | Hops are added into unfermented beer to extract bitterness and create flavor/aroma                                                                                                                                              | $39.1-67.8 MJ$                                                                                                                       |
| Whirlpool tank               | No heat required              | $40-80 \degree C$ | Separates the solid proteins and wort mixture from the wort mixture. This mixture is then chilled and sent to the fermenters                                                                                                    |                                                                                                                                      |
| Packaging and pasteurisation | LP steam ($130-160\degree C$) | $60-70\degree C$  |                                                                                                                                                                                                                                 | $22.4-38.9 MJ$ Note that this can be keg processing or bottle/can processing, the latter can have twice theheting of keg processing. |
| Cleaning in place            | LP steam ($130-160\degree C$) | $70-90\degree C$  | Use of hot caustic solution (2% for cleaning protein, oils and organic materials from the surface of the vessel, piping, and tubing)                                                                                            | $16.6-28.8 MJ$                                                                                                                       |
| Cooling stages               |                               |                   |                                                                                                                                                                                                                                 |                                                                                                                                      |

![[Screenshot 2026-07-29 125845.png]]

#### Waste Heat

Waste heat can be recovered from
- Condensation of steam from the hop boiler (flue gas from from the kettle at $100\degree C$)
- Spent grain ($65-70 \degree C$)
- Waste water for keg washing and CIP ($70 \degree C$)

### Technology Advancement

`Zero carbon industry plan: electrifying industry. 2018. BZE`

Large plants have several gas-fired boilers with steam production operating at $9$ bar of pressure.

| Technology                               | Use case                                                                                                                                                                    |
| ---------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Anaerobic digestion of plant waste water | This generates biogas that can displace natural gas use in the boiler, used to produce steam                                                                                |
| Operational efficiency                   | Preheating the wort to $92\degree C$ to $70 \degree C$ can reduce the length of boiling and total energy used.                                                              |
| Solar thermal                            | Firmed by waste heat to supply heat required in brewing, but may require retrofit of the plant. ~={red}It is important to understand what kind of retrofits are required?=~ |
## ~={orange}Hospitals=~

### Processes

**Energy for process heating:**
- Primarily uses natural gas for heating, for one example of a Brisbane hospital $897,000 m^3$ used in 2019 for steam and water boiler, which is equivalent to $34.1 TJ$.
	- 64% consumed by the hot water boilers and $36$ consumed by steam
- gas consumption is $0.33GJ$ per patient day
- Uses a steam and hot water boiler for heating

**Emissions for process heating:**

| Process          | Input | Temperature    | Purpose                                                                    | Share of energy and GHG |
| ---------------- | ----- | -------------- | -------------------------------------------------------------------------- | ----------------------- |
| Hot water supply |       | $75\degree C$  | Used to heat potable water and softened water, for dishwashing water, taps |                         |
| Steam supply     |       | $100\degree C$ | Sterilization and air conditioning humidifying purposes.                   |                         |
There may also be gas fueled heating and cooking in the hospital kitchens.

Note that hot water has to be supplied at $60-80\degree C$ to prevent legionella growth.

### Technology Advancement

## Gaps and potential research directions

Table 15 provides a summary of the processes that needs to be decarbonised in the various industries.
- ~={red}There is a research gap in the heating demands of commercial and service sector (61 PJ/year in 2018 to 2019)=~
- Geographically based energy analysis for the larger heating consumers across Australia would be informative (Can start from the National Pollution Inventory), but will require more detailed GIS data
- Load profile assessment of batch-orientated industry affected by plant capacity factors, shift cycles, and market demand.
- There are also a lot of industry with lower process uniformity that requires more complex methodology to analyse their heating demands and consumption patterns.
- Furthermore, although energy efficiency is one of the top strategies for carbon emissions reduction, there are not enough literature to support energy efficiency improvements in the Australian manufacturing (such as through pinch analysis)

## Technologies by TRL Levels

Focus has been placed on process heat applications from $95-250 \degree C$ 

| Fuel                        | Current Price (2021) | Barriers                                                                                                                                                                                                                                               | Future steps                                                                                                                                                                                                                                                             |
| --------------------------- | -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Green Diesel                | $74/GJ               |                                                                                                                                                                                                                                                        |                                                                                                                                                                                                                                                                          |
| Green Hydrogen              | $50/GJ               | Natural gas pipelines are able to store months of energy demand and up to 20% hydrogen mix.                                                                                                                                                            |                                                                                                                                                                                                                                                                          |
| Green methane               |                      | Can be injected into gas grids without any concentration limits                                                                                                                                                                                        |                                                                                                                                                                                                                                                                          |

| Technology                   | Barriers                                                                                                                                                                                                                                                                                                                                                                                        | Future steps                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Adsorption Heat Pumps        |                                                                                                                                                                                                                                                                                                                                                                                                 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Absorption heat pumps        |                                                                                                                                                                                                                                                                                                                                                                                                 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| High temperature heat Pumps  | The use of heat pumps are limited by the refrigerant limit (critical temperature). Furthermore, solenoid valves, lubricating oils and other instruments have to be rated to the condensation temperature for high temperature heat pumps to be viable.                                                                                                                                          | What are the stage of development of new high temperature refrigerants such as HFO-1336mzz-Z which has a critical point of 171? Currently ammonia systems can deliver up to $100 \degree C$, CO2 can reach $120 \degree C$, and HFOs can reach even higher temperatures. Higher compression ratios and thermodynamic cycles can allow even higher temperatures to be reached.                                                                                                                                                                                     |
| Open cycle MVR               | High purity of water required for MVR, and requires 6 stage recompression for a temperature lift of $50 \degree C$                                                                                                                                                                                                                                                                              | It is proven in the dairy industry, but need further development                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Thermal Vapor recompression  | Uses high pressure motive steam inside a jet ejector to capture, mix, and recompress lower pressure waste vapor. More suitable for low boiling point rise liquids and low to medium temperature differentials.                                                                                                                                                                                  | Quite developed, especially in the dairy industry. It has no rotating parts and low capex and available in various industrial sizes.                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Low temperature heat pumps   |                                                                                                                                                                                                                                                                                                                                                                                                 | Additionally, work in compression improvements can bring the capacity of heat pumps higher as well as COP.                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Heat exchangers              | At higher temperature, the mechanical strength of the material drops (especially at above $600 \degree C$)                                                                                                                                                                                                                                                                                      | Current maximum temperature is $1500 \degree C$ at 2 bar. Very high TRL. There are works being done on regenerators and heat exchangers that are cheap and readily available for high temperature processes.                                                                                                                                                                                                                                                                                                                                                      |
| Electric Boilers             | Although it has a lower COP, electric boilers are easier to integrate compared to heat pumps are also low capex to enable the                                                                                                                                                                                                                                                                   | It is not only electrode heating, infrared, microwave, and radio frequency heating are also available on the market. However, the efficiency of these systems are lower, from 50-70% for microwave heating to 40-60% for IR gas heating and radio frequency heating.                                                                                                                                                                                                                                                                                              |
| Evacuated tube solar thermal | Higher efficiency evacuated tubes and solar concentrating systems are required. Newest evacuated tube systems achieved 60% efficiency when delivering steam of up to $200\degree C$. Fresnel solar thermal can reach up to $400 \degree C$.                                                                                                                                                     | Solar thermal delivering up to $250\degree C$ with trough and linear fresnel systems have generally been well established. However, very location dependent due to irradiance requirements                                                                                                                                                                                                                                                                                                                                                                        |
| Biogas and waste combustion  | Note that biogas is used in commercial use and needs to be upgraded into bio-methane for use in C&I. Capacity for biogas combustion is concentrated in the US, Germany, and China. The share of bio-methane is increasing in the transport sector. However, upgrading biogas also produces $CO_2$, which can be stored underground or used in industry to produce more steam or for greenhouses | Where biogas is methane, CO2, and water vapour mixture, bio-methane is a highly refined product. The former is much less energy dense and can be scrubbed or membrane separated to obtain higher purity bio-methane. Bio-methane is completely indistinguishable from natural gas and there is no limit to injection into the gas pipeline. Note that there is a push to move biogas to CHP, which has a higher energy efficiency. Still working towards gasification of biomass to directly get bio-methane. Currently the use if 3% of the total energy demand. |
| CSP                          | Cannot achieve lower capex compared to wind and solar and can lend themselves to peaking services. It is also more economical to sell the biogas                                                                                                                                                                                                                                                | Value proposition for specific C&I application needs to be made.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| TES                          | These systems can be sensible (just by changing temperature), latent, or thermochemical systems. Some thermochemical systems can reach up to 1800$\degree C$, but then we need to consider the integrity of the materials.                                                                                                                                                                      | Pretty advanced in commercial scale thermal energy storage systems that can store at temperature of >$600 \degree C$. Lower duration than energy storage. However, industrial processes may only need a few hours on storage, in which case conventional steam accumulators are sufficient                                                                                                                                                                                                                                                                        |
| BES                          | Due to induction heaters being able to deliver the same heat for less losses, BES may be more cost effective than TES, and can also provide longer storage durations.                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Direct Heating               | Target material needs to be homogenous                                                                                                                                                                                                                                                                                                                                                          | By changing radio frequencies, non-homogenous objects can be heated uniformly. Microwave conversion efficiency also increased by using silicon carbide as a target material for heat pyrolysing, reaching an efficiency of 65%. The target material reached 1000$\degree C$ in less than 10 mintues.                                                                                                                                                                                                                                                              |
| Solar Thermal                | Solar thermal can be firm                                                                                                                                                                                                                                                                                                                                                                       | Recent works involve coatings to improve absorptivity, integrating reflectors, heat pipes or TES and developing advanced working fluids. Future technologies may reach higher thermal efficiency at higher temperatures.                                                                                                                                                                                                                                                                                                                                          |
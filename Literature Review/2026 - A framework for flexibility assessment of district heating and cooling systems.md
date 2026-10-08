https://www.sciencedirect.com/science/article/pii/S0306261926006252
## Contributions

## Content

#### Electricity Consumption Response

The change in consumption of energy between a variable price and fixed price scenario. However, this reflects a net volume change of energy export or import.
- Future metrics could price weight the flexibility provision to differentiate between scenarios based on economic significance of consumption shifts.
#### Peak Load Adjustment

Measures how the system's peak electricity demand varies between variable and constant price conditions. This is particularly relevant for grid stability and demand side management

- Shows that there are coupling between congestion and flexibility (i.e. the grid metrics concerning grid operators)

Does not capture peak shifting, shaving or increasing behavior outside of price peak

#### Operational Flexibility Range

The electricity and thermal consumptions per year under 60 scenarios (15 scenarios and 4 years) are characterised in a scatterplot which shows how electricity consumption level and dispatch can vary under different modes.

#### Thermal Generation Utilisation Rate

Capacity factor of the aggregate thermal generation to understand if there are upward mobility for flexibility.
- You would want this figure to be in the middle of the pack as extreme values limits flexibility in one direction

#### Storage to Peak Ratio

Measures how many hours the storage can supply thermal demands at peak storage. However, the charging strategy will determine the usage of the storage. 

#### Thermal Storage Utilisation Factor

Measures the total charging and discharging activity relative to the maximum possible throughput for all storage technologies throughout the year. This is then normalised against the maximum throughput.

- A high TSUF indicates frequent usage, while a low value indicates untapped flexibility potential

#### Other indicators used

- LCOH
- ~={green}Electrification Share: Capacity of the network that relies on electricity for heat generation=~
- Carbon intensity of thermal energy $kgCO_2/MWh-th$

### Simulations

- Generated price scenarios from different generation mixes using the GENeSYS-MOD. This is fed into the stochastic portfolio optimisation model

- Thsi stochastic portfolio optimisation model determines the cost-optimal heating and cooling supply technology portfolio at the district level.
	- The objective function minimises the ttoal cost of DHC
	- Models 7 heat generation systems, 3 cooling, generation technology, and 3 TES systems (Including borehole, ice, and tank thermal storage)

The study looks at 15 scenarios with unique energy demands, prices, regulatory measures.
- One of these variables is hotter summers 
- Considers flexible electricity market in one of the scenarios, where prices are strictly non-negative due to other market participants
- As the simulation is doen over 4 years, comparisons can be made of the system over the temporal dimension to identify how the flexibility evolves alongside system expansion and technology deployment. 

These scenarios impact dispatch, rather than investment scenarios.

The proposed method is done for a small district in Trondheim, Norway
- It is close to an existing DHC network, has the potential for borehole TES for seasonal storage, and can be charged by surplus heat from a nearby waste incineration facility.
## Results


## Limitation

The author highlights that the framework thresholds (benchmark values for the metrics) will have to be adjusted based on available technology portfolios, grid characteristics, local climate conditions, and prevailing market structures.
- Again, the paper does not attempt to relate network characteristics to performance metrics

Hourly simulation resolution mean that it excludes sub hour ancillary services



https://www.scopus.com/pages/publications/105005501552?origin=resultslist

This was a shit paper, inconclusive to the design variables in heating production networks.
## Contribution

This study aims to design an optimized 5th-generation district heating and cooling (5GDHC) system that balances investment costs, operational expenses, and CO2 emissions while integrating renewable energy sources effectively.
- Responds to tightening environmental legislation and rising fossil fuel prices.
- However, the study does not actually use carbon emissions as a KPI. Rather, lower carbon emissions was just a by product of designing a more efficient 5DGHC. (The figure isn't even mentioned in the paper)*

Some of the questions that the paper tries to answer is
- How does outdoor temperature affect heating and cooling demand for different building types, and how does that affect the design of the heat production network.

Rather than using bottom up data of individual space heating needs and thermodynamic calculations from first principle, the study uses a top-down approach that uses
- GIS inputs. The use of GIS enables better correlation of spatial limitations, weather constraints, network topology, and building energy demand with the design of the heat production network. Further, the study places a heavier focus on the impact on seasonal variation on heat production network variation. Comparatively, MILP may linearise non-linear behaviours and create complexities in more convoluted system design.
- Historic weather data
- Building energy demand data, considering heat demand, network layout, and temperature requirements. Noise is introduced into the energy demand data for stochastic variability.
	- Note that buildings are aggregated to $1GWh/year$ cluster to reduce simulation complexities.

The current study places greater emphasis on local historical weather data, particularly outdoor temperature, which is a key driver of energy demand. This simplification ensures that the network configuration remains adaptable to different environmental conditions without the need for detailed energy flow data at the hourly timescale.
- Review of literature also shows that climate impacts the temperature of waste heat (e.g. temperature of tunnel air in the underground metro system). The study looks at a data centre as a seasonally varying heat load.

A case study area, including more than 108 office buildings and three data centers as waste heat sources, was used to test the tool.

#### Control strategy

In terms of control strategy, opts for simpler rules based control strategy, which is still effective without more complex implementations of MPC.
- For the battery charging strategy, the TES charges when cooling demand is lower than the heating demand and discharges when vice versa. However, this does not consider time of use pricing of energy.

## Content

In most heat production networks, poor planning of district heating networks means that operation cannot adapt to more extreme climate scenarios, increasing energy demands, and changing efficiency requirements.

- The application of GIS to energy systems in relatively new?
	- Ensures that heat production network adheres to city constraints such as streets and building placements.
	- The use of GIS also allow for incorporation of humidity, wind speed, and other local factors that affects a building's energy needs. But this not done in this study
	- GIS is used to find the heating demand based on surface area.

The network topology was chosen through a MST algorithm that considers the cost constraints and environmental impacts (minimise emission and maximise renewable energy)
- Using the constraints and inputs, the tool was able to figure out the optimal mix of technology
#### Network expansion

In stage 1, the network connects at least one data centre, one office building, and a TES unit into the network. Then the expansion can be formulated as an optimisation problem where the cost has to be minimised whilst meeting demand.

- In the expansion scenarios, each scenario evaluates the impact of adding new buildings, adjusting pipeline routes, or incorporating new waste heat sources on overall system efficiency.

Cost ratio (CR) $$CR = \frac{\text{5GDHC System Cost}}{\text{Reference System Cost}}$$ is used as a KPI for determining the economic efficiency of the 5GDHC system that will be implemented 

The minimal network topology is found using a minimum spanning tree algorithm and the pipe diameter determined by the peak heating or cooling load. As the peak heating or cooling load is dependent on the mass flow rate in the supply lines. (in case of high peak demand, there will be a high mass flow rate and a high pressure drop to achieve this. Subsequently, the diameter of the pipe will increase if pressure drop increase beyond acceptable threshold.)

## Results

There is one conclusion which can be drawn from this study, which is the the impact of climate on building heat demand.
## Limitations 

The study suggested that the sensitivity of the system performance to different climate data and energy market signals is a significant metric of performance.
- [16] and [17] covers these topics, and this paper does not include sensitivity.

- For efficient network design, buildings with energy demand below a 1 MWh/year threshold are excluded from the layout to avoid unnecessary infrastructure. However, this limits network design from the outset and should be left to the optimisation engine.
	- The connection of these smaller heat pumps may serve auxillary functions that are not considered under the current key performance index. And this threshold is also different in different countries. What is the impact of changing the connection threshold?

- Neglected heat loss in the transferring heat from the network temperature and the use temperature.

Does not talk about the grouping of asset classes to balance peak load demands.

In the end, the paper did not conduct a comparison of what makes a good heat production network.
- Considers only space heating and cooling

Ultimately, this paper only investigates, through the GIS software and given data, how load varies based on asset class, outdoor temperature.
- There is limited commentary on the design process of the heat production network

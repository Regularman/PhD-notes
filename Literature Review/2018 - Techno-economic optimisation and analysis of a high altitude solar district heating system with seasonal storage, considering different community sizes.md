https://www.sciencedirect.com/science/article/pii/S0038092X18300732?pes=vor&utm_source=scopus&getft_integrator=scopus

## Contribution

Answers the question of how much demand a solar thermal district heating system can provide for, simulating solar thermal and solar electric panels in TRNSYS. Finding the efficiency of scale at a large scale. Tested at community sizes of 50, 100, 200, and 500 buildings
- Also includes two short term storage tanks
- seasonal borehole thermal energy storage system
- Ground source heat pump for additional energy generation.
This study tries to answer the question of high seasonal variability and conductive ground in high altitude communities in Finland. This fits into the larger trend of 

Optimised with a genetic algorithm using the MOBO optimisation tool. The objective function was a multi-objective optimisation function looking at life cycle cost and energy performance. 

Ultimately found that large communities rely less on heat pumps, as they utilised more on the direct utilization of seasonally stored heat. In the best vs worst case, the electricity consumption was lowered by 80%.
- For all community size, renewable energy fraction was close to 90%, but large communities could do it at 20% of the cost
## Content

The storage tanks were kept at two temperatures for separate purposes for energy efficiency ($40\degree C$ for space heating and high temperature tank was used to boost the district hot water to a minimum temperature of $55\degree C$)

- If tank rose $10\degree$C above the set point, then the water was discharged into the seasonal storage until the tank has cooled down enough. Flowrate into te borehole could be altered to prevent the storage tank from overheating.
- BTES also offer charging when the tank temperature is too low and there is not enough electricity
	- If the temperature is not high enough in the bore hole, the heat pump can be used to boost it.
Direct electric heaters used for backup heating and grid electricity used as a backup source.

Controlled flow rate to the solar collectors to keep temperature output at $1\degree C$ higher than the top of the target thermal storage tank.

Buildings used a variety of windows, insulation, and heat recovery efficiency. Did not implement a cooling system due to low cooling needs

Space heating demand of $25-50 kWh_{th}/m^2$ and hot water demand of $35 kWh_{th}/m^2$ according to IEA data. However, there needs to be constant recirculation of water, leading to an effective use of $42 kWh_{th}/m^2$ of effective use. Space heating is variable but hot water demand remains the same over time. 

Borehole storage takes several years to heat up and achieve optimal performance, therefore the system was simulated for $4$ years and the fourth year was used to estimate the cost and performance. 

![[Screenshot 2026-07-24 at 3.36.38 pm.png|347]]

The following decision variables were used to optimise the solar community at different sizes.
### LCC consideration

Looked at the initial investment cost and operation cost for 25 years, using the Nord Pool spot price, with Finnish electricity tax and distribution price.

Does not look at the time of use on the spot market and aggregates the electricity spot market price to $12c/kWh$.

Assumed economy of scale factor for solar thermal collectors, PV panels, and the storage tanks. 

Assume cost of improving the energy efficiency of buildings. Additional insulative measures are required. This allows us to calculate the cost required to have certain level of energy/heating efficiency in the building stock.
## Result

We want to look at several indicators to see how effective this solar community is

- Solar fraction. Uses renewable energy fraction instead as electricity is required for the operation of the ground source heat pump. This is defined separately for heating and electricity.

The profit of the PV sold off did not affect the net energy balance.

### Trends 

- Large seasonal storage volume associated with low performance (maybe because only 4 years were simulated)
- BTES efficiency is higher in large community sizes when imported electricity is high. However, there is a lower correlation at less total imported electricity (when the renewable energy fraction is high). Note that $\nu_{BTES} = \frac{E_{discharge}}{E_{charge}}$. This means that a lower efficiency can be caused by less discharging or more charging.
	- A efficiency greater than $1$ means that the solar heating system is undersized and heat pumps drain so much energy that it cool down to the temperature of the ground. When this happens, the BTES naturally regenerates
	- Shape of BTES also matters, when height to width ratio was high, the system performance was poor. A wide shape has the advantage that more boreholes can be installed, which can increase the total flowrate
	- Larger communities does not require as much borehole seasonal storage due to the larger availability of solar. Also boreholes are more expensive for larger communities. However, the paper showed that performance increased as boreholes increased. Conversely, borehole length decreased as efficiency improved, which implies that there are many shallow boreholes in a wide area.
## Questions

- From a life cycle perspective, if you never use the heat pumps, then its eco-effectiveness goes down. But we need to consider it from a systems persepctive
## Limitations

- Does not look at the planetary boundary
- Does not consider time of use in spot market pricing.
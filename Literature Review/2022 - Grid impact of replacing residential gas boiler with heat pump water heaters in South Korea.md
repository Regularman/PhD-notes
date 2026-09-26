https://www.sciencedirect.com/science/article/abs/pii/S019689042600926X
## Contribution

Looks at electrification of heat demands through heat pumps and its impacts on the South Korean peak energy demand.
- The paper then suggests to resolve this issue through using TES, comparing two different operating strategy and under different total storage capacities ($50GWh$, $100GWh$, or $200GWh$). The two scenarios examined in this study were 
	- **Scenario 1:** Charge in the morning ($0000-0600$) regime which is inflexible to forecasted demand
	- **Scenario 2:** Demand based regime which forecasted heat pump loads to charge off-peak periods

Note that peak periods is defined as the top $10\%$ of demand.
## Content

The study first estimated heat demand from gas network data and district heating information provided by South Korean district heating company.
- This was used to show a relationship between temperature, type of day (weekend/weekday), and time of day with heat demand
### Results

Showed that Scenario 1  was not as effective at reducing the peak demand on the electricity grid. 

![[Screenshot 2026-09-27 at 6.50.33 am.png]]
![[Screenshot 2026-09-27 at 6.51.37 am.png]]

Ultimately, up to 6% peak demand reduction could be achieved using a $200GWh$ TES with the demand specific charging regime.
![[Screenshot 2026-09-27 at 6.53.14 am.png]]

Furthermore, the second regime will cause lower peak demands caused by the heat pumps.

![[Screenshot 2026-09-27 at 6.54.21 am.png]]

Note that the study focuses on lower temperatures due to correlation with higher heat demand. However, the study only provides an average winter's day, rather than the highest demand day, which is what the system is designed for
- You can be designed for base load or for peak load, what is the trade-off? Another study can look at trade-off between using NG for peak or over-capac
## Limitations

TES is modelled as a single unit, instead of being distributed.
- This ignores additional distribution loss associated with charging the thermal battery
- Furthermore, geographical distribution of load and load profile will likely affect peak demand periods.
- Furthermore, the modelling ignores the COP variations of the heat pumps throughout the day
- Does not model thermal stratification or interaction with other renewable energy sources
- 
https://www.sciencedirect.com/science/article/pii/S2667113124000214

## Contribution

Looks at the design choices inherent in the oversizing of the solar thermal panels for different industrial load profiles, using LCOH as the performance indicator to evaluate how much the system should be oversized.

The main tradeoff is between solar fraction and system oversizing. Oversizing the system increases CAPEX and decreases yield but increases solar fraction and improves economy of scale, and affects the LCOH of the system ~={green}(for different load profiles)=~! The LCOH is therefore a tradeoff between the rate of decreasing specific yield rate and increasing solar fraction.

TRNSYS simulations are performed to simulate these solar thermal systems under different heating profiles. A under-over sizing factor of $0.5-3.5$ is used to understand the effect of over or undersizing the system (relative to the VDI guidelines that uses summer heat demands to calculate the sizing of the system.
## Content

The study highlights references the IEA SHC report , outlining that low fuel cost and high capital cost of ST systems are counteracting the requirements for low payback periods.
- It is advantageous that solar thermal system can only address parts of the peak load, as it is not necessary to design it to meet peak loads, as this would result in a considerable increase in cost and complexity. It is obviously not intuitive that the system be oversized due to low utilisation during periods of low demand that can cause overheating (stagnation). Investment can be more efficiently allocated to flexible energy sources

Recent work by the same authors highlight that 60% of 800 reviewed companies have enough roof space to meet at least the summer demands. From this we can identify the economy of scale.

![[Screenshot 2026-11-04 at 3.27.25 pm.png]]

As the collector area increase, the storage loss will also increase, causing a diminishing specific yield of the solar thermal system.

![[Screenshot 2026-11-04 at 3.54.12 pm.png]]
![[Screenshot 2026-11-04 at 3.56.46 pm.png]]

|                              | Specific Solar Collector Yield                                                                                                                                                              | LCOH                                                                                                                                                                                                                                                                                                                                      | Solar fraction (%)                                                                                                                                                                                                                                                                                                                           |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Intraweek variability        | Reduces the specific yield as there are several days where there are no heat deamnd.                                                                                                        |                                                                                                                                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                                                              |
| Increasing oversizing factor | ![[Screenshot 2026-11-04 at 4.00.02 pm.png\|200]]In general, less seasonal profiles are more sensitive to oversizing yield decreases. This is as oversizing can address winter heat demand. | However, for the given load profiles, only (0,1) has its optimum at an oversizing factor fsol,sim of 1. An increase of the collector area by 25 % only results in a minor increase of the LCOH, whereas 50 % oversizing increases the LCOH by 1 €-Ct/kWh, which still is a small increase compared to the absolute level of LCOH (+ 6 %). | ![[Screenshot 2026-11-04 at 4.09.02 pm.png]]Solar fraction increase with oversizing of the solar collectors. For loads with higher seasonality, oversizing impacts is significantly mitigated. This is although solar penetration increases in winter months,  the specific yield decreases, leading to counterbalancing of solar fractions. |
|                              |                                                                                                                                                                                             | In the other cases, the LCOH are even slightly lower when the collector area is oversized, because the specific costs decrease faster than the specific yield. The optimum lies at a value of fsol,sim of 1.25 for all the load profiles but (0,1).                                                                                       |                                                                                                                                                                                                                                                                                                                                              |
Further, as the cost efficiency curve falls flat at higher heat demands, the authors the theorise that the case for oversizing will become negligible at higher heat demands.
![[Screenshot 2026-11-04 at 4.25.04 pm.png]]
The deviation of the LCOH between the VDI 3988 design and an overdimensioning of 50 % are nearly negligible for all scaling factors 1, 5, and 10 GWh/a. It can therefore generally be concluded that an oversizing of up to 50 % with the associated increase in the solar fraction is possible without significant economic disadvantages
#### Assumptions

The storage level is determined to be $100L/m^2_{gr}$ based on VDI methodology.
There is also a backup system, so that the solar thermal system is evaluated as part of a larger hybrid system rather than as a standalone system. To ensure economic viability, this backup system(CHP or heat pump) has a minimum of 5000 operational hours.

No reference system is used.
VDI2067 provides methodology to evaluate the annuity of the ST system. The annual interest rate is set to 6%, with a project lifetime of $20$ years. 

## Limitation

Does not consider the increase in cost due to the increase in storage volume, as it only uses specific costs from the empirical data.

The study also fixes the return and supply temperature at $80\degree C$ and $60\degree C$ and therefore discounts the impacts of ambient temperature on the supply line.
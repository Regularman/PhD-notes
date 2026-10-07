https://www.sciencedirect.com/science/article/pii/S0306261921002014
## Contribution

Models the performance of an industrial district made up of a hotel, dining-bar, residential, museum, office, retail, warehouse (each with its own load profiles), which is supplied by a bidirectional heat pump connected to an anergy network.
- The system is optimised for NPV under different variables (with/without energy sharing, TOU/fixed rate tariffs, with/without carbon saving tariff). This produces 16 unique scenarios
- The optimal equipment size (of heat pump (both hot and cold size)) and TES is chosen in each scenario

Further, the paper assesses the suitability of each building type for connecting into an energy sharing network. The novel contribution of the paper is showing complimentary heat loads based on load profiles through a load matrix.

This study begins to answer how characteristics of the system (in this case load profiles) affect the design of the heating network. For example, it outlines how different load types are complimentary to energy sharing. However, the study focusses on the energy sharing % metric, although this can be related more to the grid or cost metric, which would make the analysis more relevant.
## Content

Note that in an energy sharing network , when the hot side heat pump operates, the supply fluid leaving the evaporator will be cold, and this will be used to charge a cold thermal tank or be used in the cold side process.

The metrics used to analyse the benefits from energy sharing are shown in the table below

| Metric                 | Description                                                                                                                                                                                                                                                                                                                                                   |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Diversity Factor       | Since it is unlikely that all of the users' peak demands will occur at the same time, the diversity factor is defined as $$\frac{\text{Peak Energy Provided from a production plant}}{\sum \text{Peak energy demand of end users}}$$Thus, an increased diversity factor will reduce the installed capacity of production equipment and distribution agreement |
| Floor Normalised Loads | The normalised load of each building according to floor space, fit to a particular profile. This is used to develop the load matrix used to compare complimentary use cases.                                                                                                                                                                                  |
| LCOE                   | $$\frac{CAPEX+OPEX}{\sum_{\text{lifetime}}E}$$                                                                                                                                                                                                                                                                                                                |
The study looks at a city centre in England, simulated in Integrated Environmental Solutions, a thermal simulation tool, with a typical weather file for Glasgow.
#### Results - Influence of Tariffs and tax on network design

Found that carbon tax was too low to induce a response on the system capacity.

Tariff structure and energy sharing will affect the hot side and cold side capacity different due to the different load requirements (cold being seasonal and there also being hot demand, which means that cold heat pump will rely much more on energy sharing)

Energy sharing and TES has the benefit of
- reducing CAPEX from reducing installed capacity through peak shaving
- reducing operating cost when there is a variable TOU tariff or carbon tax,

~={red}The study found that there is a maximum point of benefit for shared heat. However, this does not make sense as the study does not make clear the mechanism of why WASTING shared heat is good? Unless there is a cost to sharing energy?=~

The greatest reduction in carbon emission reduction is expected to come from the presence of energy sharing, then TES, then carbon tax. However, if we look at economic metrics, energy sharing does not make a significant impact on the LCOE. The biggest impact on LCOES is thermal storage
- ~={red}Including the embodied carbon of equipment might change how the system is configured (as the study admits)=~

Thermal storage and energy sharing is required to achieve the lowest LCOE, although the former is much more significant.![[Screenshot 2026-10-07 110749.png]]

Although tariff structure does not promote energy sharing, it was found that the availability of TES promotes energy sharing (82% with and 40% without due to lack of simultaneity between heating and cooling)
- However, energy sharing did not have significant influence on NPV or LCOE.

Further, it was found that TOU tariffs have the largest impact on operating strategy. ~={red}(It would be interesting to understand the sensitivity of varying the TOU tariffs)=~
#### Results - Complimentary loads

![[Screenshot 2026-10-07 111253.png]]

The study compares different combinations and permutation of building use types on how well they complement each other, based on % of shared energy used. For example, if shows that office heating and office cooling wastes $92$% of the potential shared energy.
- This wasted energy is because there is not enough of a demand for it, leading to the energy being curtailed. Most of it is due to shared cooled energy (there is always a heating demand, but not always a cooling demand)

However, can we guarantee that this behavior will be the same when we add in a larger diversity of load?
- Further, as more building connects, then heat density may decrease, increasing thermal losses.

~={red}If energy sharing is not a significant factor for economic metrics, how is it a useful indicator of complimentary profile?=~
## Limitations

The study is static, and considers the end users demand to be in the same space, ignoring the effect of hydraulic lag in the network. This means that heat exhausted by a user can be immediately used by another user, ignoring the spatial dimension. Further, it is unclear whether and how the rejected heat will change the temperature of the network.
- As the study is static, is does not consider the minimal flow rate, grid temperature, and hydraulic lag integral to the operation of any shared energy networks.
- Further, it does not model secondary distribution
- The COP used for heat pump is also static throughout the year at a value of $3$
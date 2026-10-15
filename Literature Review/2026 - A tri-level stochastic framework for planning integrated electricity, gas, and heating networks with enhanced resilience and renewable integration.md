https://www.nature.com/articles/s41598-026-43763-7

## Contributions

The are three levels to the optimisation hierarchy proposed in this paper
1. The upper level searches for optimal capacity expansion for lines, pipelines, and conversion technologies (CHP, P2G, heat pumps)
2. The middle level solves for minimum operational cost problem under ordinary stochastic conditions
3. The lower level deals with the maximum load restoration in N-k contingencies by a quantitative resiliency measure
The tri-level hierarchal approach is interesting. Standard analysis that combines operation and resilience makes economically inefficient decisions as it assumes that the system is always under duress. Systems that are operated with resilience as an ad-hoc metric is blind to the operational state (generator commitment and storage SOC).

Resilience is defined in equation 3s as $$\phi^{resil}_{t, dis, op}=\frac{\sum \text{zone criticality factor} \times \text{load restored}}{\sum \text{zone criticality factor}}$$
Where load restored is based on the dispatch and network flow of generators on the electrical subsystem. Therefore, this paper does not comment on the construction of heating networks for network resilience.

The innovation in this study is that it proposes a resilience metric that is co-optimised with economic objectives. This will therefore use resilience as a central metric for planning of Multi-Carrier Energy Systems (MCES)
- The study will look at the economic, operational, and resilience trade-offs 

Also compares their integrated hierarchal method with the sequential method to show improvements in resilience.
- Highlights that Benders Decomposition (commonly employed in related research), is outperformed by C&CG, which is Column and Constraint Generation algorithm. BD is on one hand weak and on the other hand invalid due to the non-convexity of the subproblem.

The study also highlights the difference between operational variability and extreme event response (High-Impact-Low Probability Events)

Finally, the study also conducted empirical validation and policy implications through application of resilience design framework on a prototypical MCES.
## Content

##### Investment framework

Aims to reduce the discounted sum of all relevant costs over the planning horizon, subject to the adequacy, reliability, and resilience of the system.

#### Operational optimisation model

Optimises generation dispatch, network flows, and storage in all operational scenarios, seasons of the year and representative hours. The objective function minimises total system cost of operation.

#### Resilience optimisation

The reliability criteria used is 
- Disrupted energy
- Switching and black start procedures
- Ability to recover CRITICAL areas (recovery ratio after a disturbance causing outage of the electrical network)

The total resilience index for each time and disruption scenario is then derived as the weighted average of the restoration rate at the zone level by using the zone criticality (priority factors) as the weighting scales.

The algorithm finds the lowest cost way to recover capacity after system disturbance. The cost of disturbance events are weighted by their probabilities. The costs associated with system restarts are 
- electrical, gas, and heating load curtailment penalties
- Network switching and reconfiguration costs per energy carrier, 
- Black start costs for de-energized islands and resilience penalties associated with unserved energy in critical zones

Further, loads are given criticality weights which impacts the decision about load shedding during disturbance events.

One of the main relationships that the model draws on is impact of line contingencies and microgrid capabilities on resilience, balanced with investment costs.

In the formulation of the problem, there are two sets of equations that the study must solve, which are the 
- Attacker's maximisation of resilience system cost through binary availability variables given a budget of attack costs
- A system operator trying to minimise the impacts of disruption events through optimisation of continuous variables such as network flow and dispatch

### Results of simulation

~={red}In the simulation performed, the district heating network has set nodes and operation temperature of between $115\degree C$ to $125 \degree C$.=~
- Also does not consider the centralised, decentralised problem as the thermal network is dominated by large scale CHP, gas fired boilers, and heat pumps in the MW-scale.
- COP is also static

From the evaluation of the master problems and subproblems, the following investment pathway is shown below. One of the major issue with the modelling result is rapid increase in gas CC and CHP units in the system. This does not reflect environment/emission optimality, which is not considered in this study.
![[Screenshot 2026-10-15 114843.png|457]]

Further, the study cannot highlight heuristics surrounding heating network design. As shown in the figure below, heating network optimisation is reduced to a single variable, the heating network expansion. ![[Screenshot 2026-10-15 115113.png]]
This is further reinforced in the optimised power balance 10 yeas into the future, which shows the generation is dominated by gas generation as a baseload. In what world is an![[Screenshot 2026-10-15 120342.png]]
#### Difference in failure events
The failure events are defined by set operating scenarios
![[Screenshot 2026-10-15 114317.png]]

| Operational background failure                                       | Disruption events                                                   |
| -------------------------------------------------------------------- | ------------------------------------------------------------------- |
| Variability of renewable energy production                           | Natural disasters and HILP events that degrades system performance. |
| Energy demand at different levels of maturity in all enegry carriers |                                                                     |
| Component availability in operations in the field                    |                                                                     |
![[Screenshot 2026-10-15 114100.png]]

Therefore, the disruption events are non comprehensive and does not relate to the set up of the MCES.
## Limitations

The system design designs the heating and electricity capacity to equal that of the peak demand, multiplied by a reserve margin. This counters the point that economic investment in existing models are wasteful.

The paper imposes another restricting condition, which is the geographic diversification on generation expansion to impose a minimum amount of local generation at each zone with respect to its load to prevent too much spatial concentration of capacity. This may not reflect initiatives such as the REZs in the NEM.

Further, in operation optimisation, the equation ensures that there is enough upwards and downwards reserve in demand to receive excess power.

The study also guaranteed a minimum resilience level, restricting the overall resilience index of the system to ensure that it is never lower than some prescribed acceptable level in any disruption scenatio.

The resilience cost used to interconnect variables is only based on electrical curtailments, broken down into hourly resolutions. $$R_w= p(failure)\times\sum \text{curtailed load}\times C_{curtail} + \sum \text{criticality weight of asset}\times C_{resil}\times(1-\text{recovered load}$$where $w$ is the operation scenario. The disruption events are calculated as expected values over each operation scenario, weighted by the hour and duration of the season it occurs in.
- Therefore, this is a major limitation as it does not directly comment on the resilience of the heating network. Rather reliability is measured primarily through recovery of the electricity network.
## Further Readings 

[7] Optimal planning approach for dairy farm micro energy systems that aligns energy and material flows.



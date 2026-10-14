https://www.nature.com/articles/s41598-026-43763-7

## Contributions

The are three levels to the optimisation hierarchy proposed in this paper
1. The upper level searches for optimal capacity expansion for lines, pipelines, and conversion technologies (CHP, P2G, heat pumps)
2. The middle level solves for minimum operational cost problem under ordinary stochastic conditions
3. The lower level deals with the maximum load restoration in N-k contingencies by a quantitative resiliency measure
The tri-level hierarchal approach is interesting. Standard analysis that combines operation and resilience makes economically inefficient decisions as it assumes that the system is always under duress. Systems that are operated with resilience as an ad-hoc metric is blind to the operational state (generator commitment and storage SOC).

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
## Limitations

The system design designs the heating and electricity capacity to equal that of the peak demand, multiplied by a reserve margin. This counters the point that economic investment in existing models are wasteful.

The paper imposes another restricting condition, which is the geographic diversification on generation expansion to impose a minimum amount of local generation at each zone with respect to its load to prevent too much spatial concentration of capacity. This may not reflect initiatives such as the REZs in the NEM.

Further, in operation optimisation, the equation ensures that there is enough upwards and downwards reserve in demand to receive excess power.
## Further Readings 

[7] Optimal planning approach for dairy farm micro energy systems that aligns energy and material flows.



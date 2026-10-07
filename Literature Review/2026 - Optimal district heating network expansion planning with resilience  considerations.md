
https://www.sciencedirect.com/science/article/pii/S0360544226014568
## Contributions

The objective is to determine the optimal set of routes and consumers to connect to the existing DHNs from a set of possible routes and consumers, whilse considering resilience.
- The definition of resilience is that the failure of a generation unit does not affect a DHN's heat supply. The generator that is switched off is the most risky one (i.e. the largest one)

The algorithm also chooses the customers **most profitable** for the DHN. This is done through an objective function that takes into account the new customer's load, the annualised capex of pipeline construction and generator construction.

However, a network is defined as resilient is $$\text{Customer Demand}< \text{N-1 Generation in the network}$$~={red}This neglects the load profiles of the users and the fact that there may be TES in the network for load shifting, which contributes to reliability. Therefore, the paper does not address the question of how technology configuration can improve heating network resilience. Further, metrics such as LOLP or EENS would be a more appropriate metric for reliability relevant to an end user.=~
## Content

Represents the DHN through a graph representation, where each node has a mass flow rate attached to it based on its heat demand and required temperature difference 
- $T_{consumer}=30K$
- $T_{generator} = 35K$

The nodes and generators are from real data, but the graph network is generated through the shortest path algorithm. 
#### Results

![[Screenshot 2026-10-07 165634.png]]

We can see that in the non-resilient case, which does not consider if a generator fails, then there is no influence on the customers added.
- However in the resilient case, it requires increasing the weighting of the consumers to enable a new generator to be built

![[Screenshot 2026-10-07 170213.png|175]]
## Limitations

Reliability of a network is inherently dependent on its time coincident loading. Therefore, static simulation of the network cannot determine the network resilience during operation. 

The paper highlights that a new generator being built is never optimal. However, there are no other way to bring in new consumers to the district heating network. The focus on transitioning end user load should be to decarbonise the heat supply. In order to do so, generations must be expanded to meet the new demands.
- Most likely, this paper comes from the perspective that 
## Further Readings

[7] Price collecting Steiner trees, which selects consumers worth adding to the DHN based on node attributes
[13] also does this through a MILP approach rather than a graph approach

[16] A MILP approach is used to optimise the operation and design of a DHN simultaneously?
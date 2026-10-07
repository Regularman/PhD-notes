
https://www.sciencedirect.com/science/article/pii/S0360544226014568

## Contributions

The objective is to determine the optimal set of routes and consumers to connect to the existing DHNs from a set of possible routes and consumers, whilse considering resilience.
- The definition of resilience is that the failure of a generation unit does not affect a DHN's heat supply. The generator that is switched off is the most risky one (i.e. the largest one)

The algorithm also chooses the customers **most profitable** for the DHN. This is done through an objective function that takes into account the new customer's load, the annualised capex of pipeline construction and generator construction.

However, a network is defined as resilient is $$\text{Customer Demand}< \text{N-1 Generation in the network}$$This neglects the load profiles of the users and the fact that there may be TES in the network for load shifting, which contributes to reliability. Therefore, the paper does not address the question of how technology configuration can improve heating network resilience. Further, metrics such as LOLP or EENS would be a more appropriate metric for reliability relevant to an end user.
## Further Readings

[7] Price collecting Steiner trees, which selects consumers worth adding to the DHN based on node attributes
[13] also does this through a MILP approach rather than a graph approach



[16] A MILP approach is used to optimise the operation and design of a DHN simultaneously?
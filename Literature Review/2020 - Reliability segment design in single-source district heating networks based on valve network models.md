https://www.sciencedirect.com/science/article/pii/S2210670720306831

## Contributions

DHN reliability is defines as the ratio of the heating expectation of the actual system to the ideal system heat load,

There is a trade off between the number of valves (which restricts the area of the heat zone failure) and the reliability of the network, as the valves are a source of failure in itself.

Case study is conducted on a region in China, which has a heat load of 314.08 MW.
## Content

Note that as the heat load is split up into reliability segments, the total load $Q$ is irrelevant to the reliability metrics.![[Screenshot 2026-10-13 105433.png]]

Also investigated the effects of loading distribution on looped networks and found that extreme linear distributions of $q_i$ and $l_i$ slightly improves reliability. However, the nonlinearity degree of pipeline models is irrelevant and not considered in this study.

#### Changing the length of the network

![[Screenshot 2026-10-13 110053.png]]

![[Screenshot 2026-10-13 110109.png]]

Here we can see that the total length of the network will decrease the reliability, and that increasing the number of reliability segments have diminishing returns, due to the tradeoff between reliability and segmentation as mentioned earlier in the paper. 

Comparatively, we can also look at a looped network, which have higher reliability due to inbuilt structural reservations. Further, there is not decline zone in increasing the reliability segments due to the looped nature of the network.

![[Screenshot 2026-10-13 112157.png]]![[Screenshot 2026-10-13 112206.png]]

The design rule derived for looped network is 

- Rule 2: More heat loads should be concentrated as much as possible within shorter reliability segments through the adjustment of valves.
#### Changing $a$ and $b$, the steepness of linear variation of $q_i$ and $l_i$ on the branched network

The value of $a$ and $b$ were varies int he range $[-0.66, 0.66]$, forming a reliability surface when $L$ and $v$ is fixed.![[Screenshot 2026-10-13 110946.png]]

It was shown that $\Delta R_a = 0.16$ and $\Delta R_b = 0.14$. Therefore, the influence of heating load distribution is higher than the length of the branch network. Further, in the figure below, it can be seen that the concavity of network distribution has nothing to with the reliability (varies very little). It only matter that the distribution is decreasing for load and increasing for distance.

![[Screenshot 2026-10-13 111452.png]]

Therefore, the design rule is that 

- Priority should be given to the decreasing distribution of the reliability segments’ heat loads from the heat source to the end of the pipeline.
- The valves aiming to improve reliability should be set at the heat outflow side of the node-connected branches, so as to ensure the reliability segment on the upstream side of each valve contains more heat loads and fewer components.

~={red}However, as other papers on the reliability of electricity network highlights, centralisation of heat loads increases the risk of congestion on the power grid.=~

![[Screenshot 2026-10-13 112615.png]]

This is the reliability surface for the looped network. $\Delta R_L = 0.07$ maximally. This is because of the looped nature of the network already having inbuilt robustness and the distribution of heat load only acts as a buffer.

## Simulation and results

It is shown that a complex heating network can be decomposed into the looped or branched networks, which allows the previous design rule to be investigated in this case study. The following heat network in China was decomposed into 
- 1 L1 main loop
- 6 B2 branches lines
- 2 B3 branches lines, and 
- 24 B4 branched lines
![[Screenshot 2026-10-13 113124.png]]

#### Design optimisation of the looped network

Compared two schemas
1. Used design rule for looped network and kept heat load high where reliability segment is shorter and vice verse. Achieved reliability of 96%.
2. Contradicted design rule and kept heat load low where reliability segment is low. Achieved reliability of 92%.

![[Screenshot 2026-10-13 113831.png]]
## Limitations

Did not consider the failure of more than one component simultaneously. However, the number of permutations of outages will increase the probability of these lower chance events through markov modelling.

- How does implementation of TES insulate heating networks from outages?

The pipes also only have two states: intact or faulty. Does not consider where pipes are under maintenance.

Further, the analysis only considers single source branched or pipe networks, and does not investigate how multiple source and variation of loads will affect heating network availability.
- Assumes that the loads and length of the network fits a linear function, which isn't reflective of reality. By changing a and b, which are the linear coefficients of these functions, the steepness of load and length from the source can be investigated. However, this is only applicable to single source networks.


![[Screenshot 2026-10-13 104839.png]]
- They also study the non-monotonic increase and decrease of load from the source

![[Screenshot 2026-10-13 105216.png]]

With reliability, businesses care about it because of profitability. Reliability analysis will also be different in a peer to peer network compared to a single source network.

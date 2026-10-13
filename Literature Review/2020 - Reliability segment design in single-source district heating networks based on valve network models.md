https://www.sciencedirect.com/science/article/pii/S2210670720306831

## Contributions

DHN reliability is defines as the ratio of the heating expectation of the actual system to the ideal system heat load,

There is a trade off between the number of valves (which restricts the area of the heat zone failure) and the reliability of the network, as the valves are a source of failure in itself.

Case study is conducted on a region in China.
## Content

Note that as the heat load is split up into reliability segments, the total load $Q$ is irrelevant to the reliability metrics.![[Screenshot 2026-10-13 105433.png]]

Also investigated the effects of loading distribution on looped networks and found that extreme linear distributions of $q_i$ and $l_i$ slightly improves reliability. However, the nonlinearity degree of pipeline models is irrelevant and not considered in this study.

#### Changing the length of the network

![[Screenshot 2026-10-13 110053.png]]

![[Screenshot 2026-10-13 110109.png]]

Here we can see that the total length of the network will decrease the reliability, and that increasing the number of reliability segments have diminishing returns, due to the tradeoff between reliability and segmentation as mentioned earlier in the paper.
#### Changing $a$ and $b$, the steepness of linear variation of $q_i$ and $l_i$ on the branched network

The value of $a$ and $b$ were varies int he range $[-0.66, 0.66]$, forming a reliability surface when $L$ and $v$ is fixed.![[Screenshot 2026-10-13 110946.png]]

It was shown that $\Delta R_a = 0.16$ and $\Delta R_b = 0.14$. 
## Limitations

Did not consider the failure of more than one component simultaneously. However, the number of permutations of outages will increase the probability of these lower chance events through markov modelling.

- How does implementation of TES insulate heating networks from outages?

The pipes also only have two states: intact or faulty. Does not consider where pipes are under maintenance.

Further, the analysis only considers single source branched or pipe networks, and does not investigate how multiple source and variation of loads will affect heating network availability.
- Assumes that the loads and length of the network fits a linear function, which isn't reflective of reality. By changing a and b, which are the linear coefficients of these functions, the steepness of load and length from the source can be investigated. However, this is only applicable to single source networks.


![[Screenshot 2026-10-13 104839.png]]
- They also study the non-monotonic increase and decrease of load from the source

![[Screenshot 2026-10-13 105216.png]]

With reliability, businesses ca

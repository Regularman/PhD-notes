https://www.mdpi.com/2227-7390/13/23/3734

## Contribution

Considers how the capacity of installed P2H technologies and its siting (relative to the electrical and thermal load), affects reliability metrics, offering a reliability-based decision making framework.

The metrics used in this paper is the Loss of Load Probability, Expected Energy not Supplied, and Self-Sufficiency rate, which are normalised into a composite Reliability Index, used as a one stop shop to assess the reliability of a network.

A case study is done on a South Korean university campus. However, the results are not validated, and it is not understood if the designed network is actually more reliable.
## Content

Reliability is modelled by running sequential Monte Carlo simulation for alternative siting/sizing scenarios. These MC simulated results are aggregated into resulting indices into the CRI for comparative assessment.

![[Screenshot 2026-10-09 185935.png]]
![[Screenshot 2026-10-09 190038.png]]
The Monte Carlo simulation varies the capacities of the technologies and location of the heat DERs to investigate the given reliability metrics, which are aggregated over $S$ Monte Carlo runs.
- Each piece of equipment has its own failure data, which is then used to inform the reliability metrics in the Monte Carlo simulations.

Overall, study highlights that reinforcing thermal resources at the loads where the heat loads concentrate can drive LOLP_t to practically
## Limitations

However, the limitations of this study is that there are limited design decisions that affects the reliability metric. 

- Further, the outage scenarios does not consider redundancy and thermal transmission failure. This means that the topology of the thermal transmission network is not used as a input into the design and operation space.

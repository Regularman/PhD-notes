https://asmedigitalcollection.asme.org/energyresources/article/140/2/020905/372477/Topology-Optimization-of-Robust-District-Heating

## Context

In this paper, robustness is a weighted sum of first-order minimum pressure sensitivities to a fluid dynamics resistance noise.
- Optimisation is performed with a gradient based optimiser
- Proposes a method to evaluate robustness without evaluating the stochasticity of the network

In robust district heating networks, the minimum pressure head is affected by random fluctuations of the local fluid dynamic resistance, as a result of fouling, chemical depositions or valve actions needed to handle malfunctions. The objective function is $$\sum^{nb}_{i=1}\frac{d(P_{min})}{d\beta_i}w_i$$where $\beta_i$ is the sum of the local friction sources of the pipe, $P$ is the pressure vector across the pipe. The partial fraction describes change in pressure with change in local friction. This robustness metric is fully deterministic and does not rely on statistical moments
## Content

The robustness of the district heating network is inversely proportional to investment cost of the network due to the cost required to build additional looping branches.

## Results
![[Screenshot 2026-10-12 153852.png]]

The system considered in this work is a portion of the Turin district heating netwro
## Limitations

- Expects agreement with conventional robust or reliability based design approaches dealing with uniformly distributed and tightly bounded stochastic variables with a linear objective noise relation. When the variability in friction is large, $P_{min}$ may scale sublinearly and the method will underestimate the failure region.

## Further Readings
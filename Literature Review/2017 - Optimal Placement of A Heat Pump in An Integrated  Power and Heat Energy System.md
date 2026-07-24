https://ieeexplore.ieee.org/document/7923966

## Contributions

Looks at using a 400kW heat pump.

Uses nonlinear integer programming in MATLAB to minimize the investment of both electric and heating utility due to heat pump installation.
- Considers two electric main substation. Looks at which substation to connect to and how far as to optimise the investment cost
- Constrained by the transformer capacity and the transmission thermal limit
- Heat pump can only be connected to one substation

MatPower is used for power flow calculations.
- The non linear optimisation problem is solved using genetic algorithms 

## Content

### Topology of the heat network

Uses the minimal spanning tree to give the minimum length of pipes under a radial network constraint. However, this places limitation on type of network (ring networks), which can be used in the system.
- Optimisation with environmental impact will look very different in terms of network topology and the types of assumptions we can make
## Limitations

- Does not consider thermal storage and environmental impact. 

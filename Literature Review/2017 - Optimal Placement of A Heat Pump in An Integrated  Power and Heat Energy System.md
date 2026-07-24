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

Looked at scenarios where only heating utility investments are considered, where only electric utility investments are considered, and where both electric and heating utilities are considered. However, this is not very significant

### Results

Trivial results, cheapest heating utility when its closest to the heat load and cheapest electricity utility when it is closest to the substation.
When both heating and electricity costs are considered, it chooses a more middle point , showing reduction in cost.

- Shows some network impact of voltage stability and congestion of the heat pump, but this does not reflect the operational profile of the heat pump.
## Limitations

- Does not consider thermal storage and environmental impact. 
- Does not actually calculate the operational losses of the pipelines, this is assigned by a factor that represents higher losses.
- Does not consider other geographic and housing considerations that shows up in a GIS.

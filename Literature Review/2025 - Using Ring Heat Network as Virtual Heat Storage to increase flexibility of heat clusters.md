
https://ieeexplore-ieee-org.wwwproxy1.library.unsw.edu.au/stamp/stamp.jsp?tp=&arnumber=11096009&tag=1
## Contribution

Develops an optimal dispatch strategy based on virtual heat storage modelling of a ring heat network to improve heat sharing amongst clusters. The virtual heat storage is an intermediate component that engages in dispatch optimisation, coordinating between small clusters.This enables heat interaction amongst clusters and promotes energy efficiency.

The dispatch algorithm has two layers
- The top layer optimises the dispatch strategy based on VHS storage parameters
- Inner layer calculates the Ring Heat Network's operation temperature and flow based on energy interactions and updates the VHS model
This algorithm must allow for support for role-switching prosumers and adaptation to dynamic operating conditions.

This paper is a part of the study looking into Integrated Energy Systems, and the concept of prosumers.
- Microsystems may contain industrial waste heat linked to a cluster of buildings or waste heat from data centers utilised by self-prosumers.
- These clusters are selected during planning with considerations for geographical location, energy resource availability, and load matching
## Content

The paper highlights that traditional storage modelling are simplified tanks or static segments, or assume constant temperature or flow conditions. These factors limits ability to optimise scheduling where both flow and temperature fluctuates.

The introduction of ring heat networks where participants can be both producers and consumers is a variable flow - variable temperature regulation system. However, this is a non convex (Meaning that there are multiple optima) problem compared to steady state flow problems. 
- Changing boundary conditions and internal energy flow creates a couple discrete continuous problem
![[Screenshot 2026-07-01 at 4.08.41 pm.png]]
In this paper, there are multiple clusters, and we are coordinating between these clusters for optimal dispatch using the VHS unit.
- The VHS unit is built based on energy conservation principle, thermodynamics, and hydraulics constraints

Traditionally, the heat distribution network might be variable flow, constant temperature, or constant flow, variable temperature. However, with the rise of prosumers, this is turning to VF-VT problems.
### Heat network modelling

Takes the heating ring main unit and splits it into discretised models. 
- Assumes that each pipeline micro element operates in steady state within scheduling timestep (1 hour)

Note that when splitting into micro-elements, we are looking at the change in thermal heat capacity form the left to right hand side of the node. Exchange of heat between that node and the cluster will lead to a change in the mass flow rate of water. To avoid complications, we have to ensure that the cluster nodes are positioned between 2 micro elements and not within the micro-elements.

Note that water flow is injected from the cluster to the ring heating unit (through the interface between clusters and the ring unit, it needs to abide by mass flow constraints and temperature mixing model constraints)
- Temperature change is also limited

The VHS model is modelled using 4 parameters analogous to a battery
- maximum thermal storage capacity
- heat loss
- maximum heat input/output power per time period
- SOC

These are used as decision variables in the dispatch model, and must be updated in the inner loop.
- Note that the dispatch model optimises for cost

The VHS model therefore creates an explicit mathematical relationship between storage capacity and operating parameters.

### Heat flow calculations (inner loop)
Used to determine the parameters of the Ring Heat Unit at each timestep.
- When the cluster acts as a heat source, the water supply temperature is fixed at $60\degree$C and when the cluster serves as a load, the outlet temperature is $40\degree$C. 

To calculate the temperature at the end of the pipeline to the cluster, we need to determine the temperature at the beginning of the pipeline. We work backwards
- Beginning at the node temperature, then determining the downstream pipeline temperature based on the upstream node temperature, until all nodes are calculated.
There is a unique solution given the power in and out given by the dispatch model which converges towards the optimal solution.

### Optimisation model (outer loop)
The outer model optimises the dispatch strategy based on the fixed power in and out of the cluster. While the inner model updates these two power figures using the heat network calculation using the dispatch strategy. This is iteratively determined until convergence of a given threshold.
- By fixing the power in and out of the cluster, the dispatch algorithm becomes a convex problem

The paper also proves why the control loop converges towards an optimal solution.

### Case study

Jiangsu, China. It has waste heat recovery from power plants and steel mills, excess heat from data centres, and waste heat from sewage.

- Power and transmission loss cost is set at $0.04/kW 
- Scheduling time is 1 hour
- Diameter of the pipes is set at 0.3m 

Used this actual data to compare with the model and this shows close convergence. The granularity of the microelement model is strongly correlated with the error.
- Need to strike a balance between computational complexity and accuracy of the model.

The dispatch strategy is cluster based without specifying the dispatch of specific buildings. Alternatively, each building within the cluster is adopted. The clustering algorithm showed significant performance increase.
- Furthermore, individual collections means more source load nodes, resulting in a more volatile RHN

Improved self consumption from the electricity dispatch. Although the paper highlights higher volume of outflow and inflow, there needs to be better tools to analyse this data. How can we quantify how much better the VF-VT dispatch algorithm is?
- Local consumption is greatly increased to reduce reliance on the outgoing grid.
## Questions

How do I determine if a set of constraints are convex?
Learn linear programming. 

## Limitations

## Further Readings

[4] introduces the concept of data centre waste heat as a prosumer.
[5] waste heat recovery from domestic heat systems

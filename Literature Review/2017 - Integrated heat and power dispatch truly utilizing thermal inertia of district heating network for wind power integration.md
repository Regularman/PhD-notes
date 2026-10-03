https://www.sciencedirect.com/science/article/pii/S0306261917316793

## Contribution

This study looks at how a dispatch model which considers thermal inertia of the district heating network (connected to a centralised CHP cogeneration unit) in China can increase the wind power integration in the power grid. 
- However, the increase in wind power integration is not specifically quantified.

The study introduces a new integration model to represent the thermal inertia in the network system.

The study is an ex-post analysis of dispatch strategies for the CHP unit. The decision variables are 
- Electricity and heat generation in the CHP
- Integrated wind power
- Power purchased from the connected power grid
- Dynamic supply and return temperature at the DHS

These variables are optimise to solve for the objective function that minimises daily operating cost and also the wind power curtailment.
- However, the study does not explain how co-optimisation is done.
- The study compares the IHPD model (with thermal inertia), with the CHPD model, conventional dispatch model, to compare differences in wind curtailment.
## Results
![[Screenshot 2026-10-03 at 12.01.07 pm.png|463]]

Due to thermal inertia in the network, the IHPD model does not have to follow the heat load directly.![[Screenshot 2026-10-03 at 12.02.42 pm.png]]

From the results, we can see that the IHPD model is able to mitigate wind curtailment, but the extent to which is this done is not fully detailed.

One of the best features of this IHPD model is that you can optimise the supply and return temperature such that wind integration is maximised within the district heating network.![[Screenshot 2026-10-03 at 12.03.53 pm.png]]


## Limitations

Does not analyse how heating networks can be designed with this variable in mind (this will be network temperature, network length, and pipe diameter)

- Does not factor into account the fact that wind curtailment might be due to technical/thermal constraints on the power transmission line. Therefore, a decrease in electricity generation may be needed to allow more wind generation to come on line. In this methodology, CHP units turns down during periods of high wind curtailment. This means that the electricity demand met by the CHP unit is now replaced by wind energy.

Furthermore, the study is limited as it takes the the load as a centralised unit, characterised by the area heat index used in China.

Heat pumps will have a different mechanism of operation, since heat and electricity is not coupled.
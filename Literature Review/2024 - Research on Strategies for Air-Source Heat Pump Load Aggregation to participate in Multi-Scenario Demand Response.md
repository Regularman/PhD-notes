https://www.mdpi.com/1996-1073/17/11/2471
## Contributions

This paper looks at the aggregated response of ASHP for demand management, with the stakeholders being the Power System, Load Aggregator, and the Thermal Load (consumer). Three different scenarios were analysed.
- In non regulatory periods: MPC is employed, considering energy storage characteristics, user thermal comfort, time of use tariffs to minimize cost
- In regulatory periods, it considers user comfort and regulatory instructions to allocate adjustment power to loads, aiming for high profits, while controlling the aggregated power during the load recovery process to suppress large scale rebound.

The paper also considers the problem of the secondary shock from the change of demand profile.

Another consideration is that current research focuses on the start-stop operation of heat pumps, although they are of variable load.
- heat pumps are connected in series, and they can be switched on and off in certain permutations to achieve precise temperature control

## Content

Increasing market share of air sourced heat pumps in heating solutions mark them as a high quality resource for demand response in the power system.
- The main area of research of demand management with temperature controlled load focuses on air conditioning and water heaters.

One of the problems is that the aggregated control of heat pumps may disrupt load diversity and cause a significant rebound value due to unordered load recall behavior.

The paper includes thermodynamics calculation to correlate the operation of the heat pump with the temperature setpoint in the room.

### Aggregated Control

Splits into the scheduling and control tier.
- Scheduling is dedicated to the modelling of numerous temperature control loads and assessing their adjustability potential
- The control tier focuses on the collective or individual management of these loads

The load aggregator must report the load forecast curves and the adjustable capacities to the grid as the intermediary between the grid and the consumer. Whilst the grid issues peak shifting and consumption commands to the consumer.

Note that the adjustable power is determined by the temperature range that users are comfortable with (However, in the context of industrial applications, are there variance in temperature provided? For quality control, you would want the temperature to be the same every-time)
- Class 1 users are willing to sacrifice comfort for lower heating bills
- Class 2 users are not willing to sacrifice comfort

![[Screenshot 2026-06-23 142212.png]]
### Scenario 1: Non regulatory period: MPC

In this period, the aggregator need to
- minimize heating costs
- ensure user comfort

We need to combine thermal energy storage characteristic and time-of-use tariffs to allow for rational scheduling of unit activation and deactivation.
- Ultimately, the objective function is to minimise the heating costs
- The MPC method uses a rolling optimisation method instead of a one-time global optimisation method to find the optimal operating power for each control cycle

The paper contains the equations that sets up the MPC, including constraints on indoor temperature.

The control period is important!
- It should be noted that a shorter control period can lead to increased communication difficulty and damage to the heat pump
- Too long of a control interval and the indoor temperature may exceed the limits before control action is implemented (also increase computational burden)

The study uses 15 minute intervals and a 4 hour prediction window

### Scenario 2: Regulatory period

When the grid regulator sends in a signal that necessitate load side resources to participate in grid dispatch, then the Load Aggregator has to move away from the MPC strategy. Note that the control signal is calculated based on the adjustable capacity and load forecast curve published by the load aggregator.

The regulation strategy is 
- Take the two paradigm minimum of the difference between the regulation power of each regulator period and the load aggregation regulation power as the objective function. Solve that objective function so that heat pumps operate as close to the regulation power as possible
- When the target regulation power is small, we then prioritise thermal comfort. After the essential regulation capacity of the heat pump load is put into use, change the heating temperature intervals of Class II users to reduce impact of grid regulation on thermal comfort

### Scenario 3: Load recovery model

After the regulatory target has been reached and the control center disengages, the thermal load must recover back to its optimised control state. To prevent as secondary impact, power peaks must be limited to ensure a smooth restoration to the normal operating state.

The objective function in this state is to mimimise the recovery time as well as reducing the aggregated power during the load recovery stage.

To solve this multi-objective optimization problem, the paper uses a multi-objective atomic orbital search algorithm (MOAOS).
1. Candidate solutions are randomly distributed within the decision space defined by set boundaries
2. Calculate the objective function value for each candidate solution
3. With positioning being guided by a PDF, the candidate solutions are ranked based on energy levels
4. A solution set is maintained to store non dominated solutions
5. Leaders are selected from the solution space from less crowded areas
6. Positioning of the ranked electrons are updated based on energy levels inspired by electron positioning in atomic structure (Why the fuck are we doing this)
7. Above step is repeated until a specific stopping condition is met
8. A pareto front is outputted that is composed of non-dominated solutions that represent the best set of tradeoff solutions in the MOOP
## Further Readings

[5] Heat pump control using temperature setpoints
[9] Approximate aggregate model for split air conditioners, calculating their adjustability for control strategy formulation and evaluating their adjustability for control strategy formation.
[10] Thermal comfort as the basis to assess the adjustability potential of air conditioners
[12] Temperature based aggregation model capable of calculating the stable aggregated power of air conditioning loads to meet dispatch center requirements
[17] Looks at strategies to mitigate aggregated load fluctuations
There are a lot of exampled and research into air conditioning loads using aggregated controls.
## Questions

## Limitations

The model is limited as it does not integrate thermal storage into consideration, switching from direct heat pump to thermal storage operation may decouple thermal comfort/outcome with the operation of the heat pump.

Also looks at control through a centralised grid controller framework

Thermal storage is modelled as the thermal residual capacity of the building rather than any meaningful thermal storage.

Furthermore, you can consider the operation of heat pumps under a PPA.
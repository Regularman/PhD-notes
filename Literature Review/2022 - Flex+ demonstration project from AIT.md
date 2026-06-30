https://www.ait.ac.at/en/research-topics/flexibility-business-models/projects/flex

This final report is not peer reviewed
## Contribution

Individual components are connected to the component pools and send data to the pools regarding storage levels, room and water temperatures, and EV charging status.

The study implemented scalable optimization algorithms for both the prosumer and aggregator using the flex+ platform, which co-ordinates the pools and their suppliers and is responsible for aggregating and forwarding the control energy call-off signals.

1. Proposes market environments and developing business and compensation models/tariffs (work package 2)
2. And in work package 3, proposes optimisation algorithms and simulation for use cases, looking at MILP, machine learning, and MPC
3. WP-5 demonstrates these functionalities in real world projects

![[Screenshot 2026-06-30 at 12.02.54 pm.png]]
Looks at participation of aggregated heat pump in three markets

- Day-ahead spot market: Marginal pricing, all numbers get the same price, and every hour gets a different price.
- Intraday market: 5 minutes before delivery, and is pay as bid
- Primary, secondary, and tertiary reserve markets: where capacity is reserved and could be called upon. A service fee is paid for this capacity, and when energy is called up, the energy price is reimbursed, and reduced network charge in the case of a negative call up.
	- For the primary reserve, this is only for the battery pool as symmetrical supply must be given
	- For the secondary supply, if there is a deviation in the called energy with the expected value, then the next window must compensate for this for the equipment to return to the normal operating temperature
	- For the tertiary reserve market, call probability is assumed to be 0.
## Content

### Heat pump modelling

Used MILP to minimise cost for the heat pump pool. This optimiser runs on the day-ahead schedule as well as the intraday market, with the mechanisms discussed previously.

The heat pump is connected to a hot water storage tank and a building model/consumption profile.

Heat pump is described with with a empirically derived heating polynomial, depending on pump revolutions, the heat source temperature, and the outside temperature. The power range of the heat pump is specified with a binary variable.
$$Q(P(t))=\eta(t)*P(t)+d(t)*Binary(t)$$
This heating curve is calculated at each time-step. Note that there are two modes, the heat going to the hot water tank or direct to the house model. An equation constrains the overall performance with switching between the two modes.

$$\frac{P(t)}{P_{max}(t)}+\frac{P_{domestic-hot-water}(t)}{P_{domestic-hot-water,max}(t)}\le 1$$
The building is a simple capacity model (RC) represented through state space mode.
$$\dot{x}=Ax+Bu \rightarrow x(t+1)=\phi(t)x(t)+\Gamma(t)u(t)$$which represents the amount of heat supplied (heating energy, solar radiation, and internal thermal load) and the boundary temperature (ground and ambient temperature).
- Calibrated from past measurements, approximating the resulting state temperature to the reference curve at different thermal capacities and U values.

AIT partnered directly with iDM such that the optimiser information is forwarded directly to participating heat pumps.

The project optimised 4 air sourced heat pumps and 1 ground source heat pump. The heat pumps receive a new setting from a central iDM server every 15 minutes. This optimiser takes in the building's characteristic, predicted outside temperature, solar radiation, and the trend in demand and electricity prices.
- This is used to predict the demand of hot water or heating

There are some additional constraints, such as the fact that if the difference between the target and actual room temperature exceeds 1.5$\degree$C, then an additional heating phase is activated for the next 15 minutes. 

The heat pump is operating between different operating modes (hot water consumption or base heating)

### Case study: Großschönau

This is a wastewater treatment plant consisting of 2 PV systems, a battery, 2 EV charging stations, a boiler, a heat pump, and a load.
- The heat pump is used to heat the air in a room with an area of $100m^2$, which is kept at $20\degree$C to $25\degree$C. 
- While the boiler is used to supply hot water.

Data obtained from historical measurements from 2017-2019.

Ultimately found that revenue is the greatest from the secondary control market.
- ~={orange}**Furthermore, it is shown that heat pumps offer negative control energy in the secondary reserve market and positive control energy in the tertiary market. (WHY?)**. =~There is also almost no participation of heat pumps in the positive energy control of the secondary reserve market
- Comfort was defined through customer survey and questionnaires

## Limitations

- Statistically averages out case and does not do stress testing
- Overall the results in this study is quite poor in terms of presentation of data. Furthermore, the paper looks at the use of a reserve capacity mechanism that does not exist in the NEM.
- The optimiser for heating demand and hot water demand shows that there is significant overestimation of demand, and is not very effective.
	- The hot water pumps does not always behave as specified by the optimiser, and the effect of this is not discussed in its effect on energy pricing and revenue generated.
- There are only 3 heat pumps that are scheduled at a time, so the study does not look into the flexibility that aggregating many heat pumps can provide. 
- Case study from the result does not show comparative revenue with and without the heat pump participation.
- A lot of papers highlights that heat pumps cannot participate in the primary response/reserve market (60s)
- For heat pumps, they were simulated weekly and therefore showed higher revenue potential in the secondary reserve market
- The study also does not show the control of aggregated heat pumps to meet both heat demand and revenue concisely. The pool of heat pumps more so reflects a technology mix of battery. 

## Question

## Further Readings

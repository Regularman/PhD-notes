https://www.ait.ac.at/en/research-topics/flexibility-business-models/projects/flex

Written by R.Hemm and was part of the flex plus programme
## Contributions

Individual components are connected to the component pools and send data to the pools regarding storage levels, room and water temperatures, and EV charging status.
- The study implemented scalable optimization algorithms for both the prosumer and aggregator using the flex+ platform, which co-ordinates the pools and their suppliers and is responsible for aggregating and forwarding the control energy call-off signals.

Proposes market environments and developing business and compensation models/tariffs (work package 2)
- And in work package 3, proposes optimisation algorithms and simulation for use cases, looking at MILP, machine learning, and MPC
- WP-5 demonstrates these functionalities in real world projects

The aggregated heat pumps will participate in the 
- Day ahead spot market
- intraday market (5 minutes). As energy can be bought on the intraday market for one hour, it is assumed that the energy content of the pool only need to be sufficient to power it continuously for one hour. The intraday market (1 hours), is only simulated to account for the uncalled reserves in the heat pumps bidding strategy.
- balancing energy market (Frequency deviations and primary, secondary, and tertiary reserve market). 
	- In the primary frequency service case, supply offered must be symmetrical - Only applied to the battery pool for primary reserves which are 4 hour products.
	- The secondary market is a 4 hour product that takes place in 15 minute windows, Trading on the balancing energy market generates revenue through a capacity price and the energy price

The technology pooled included heat pumps, boilers, EVs, and battery.
## Content

References a base case of constant end-customer electricity tariff.

In their participation of the secondary FRR, if they get a negative call up (to consume more power), in the next window, they must purchase the positive energy demand to return the temperature to the planned level.

It is assumed in the secondary reserve market that the heat pumps are on standby.
- Therefore, is the reserve is uncalled upon, the asset must purchase or sell that electricity on the intraday market to ensure that the assets are operating within the technical operating parameters.

## Limitations

## Questions

## Further Readings
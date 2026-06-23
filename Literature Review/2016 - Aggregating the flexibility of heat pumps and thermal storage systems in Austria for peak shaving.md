https://ieeexplore.ieee.org/abstract/document/7951373

Part of the IWPP-flex program
## Contributions

Look at the application of a heat pump pool in Austria. Looks at how load shifting on the whole sale market and participating in the balancing market can reduce operational cost by 8-14%. 

This study was done in the context of residential buildings. Therefore, comfort levels was still important as an assessment criteria.

Proposes a potential operating strategy for the aggregator and technical concepts to enable signals between the aggregator and the single heat pump
## Content

We need to consider the costs of maintaining the data infrastructure required to aggregate the pool participants as well.
- Can be used for local voltage control, increasing the share of RES in the power system, to participating on the electricity market.
 Used MILP to optimise the scheduling of the pool participants.

The chosen digital infrastructure must be in line with TSO requirements.
- In case of tertiary reserve an electronic communication device is necessary to offer the minimum bid size of 5 MW in line with IEC 60870-5-101.
- Data has to be sent to the APX every 2 seconds at 50 Hz
- Guaranteed availability at 95%

## Mechanisms

External ripple control signal: Where demand services are externally switched off for demand management by utilities. This is already used by utilities with interruptible tariffs
- However, this may have a negative impact on the heat pump operation

EEBus is used for utilities or DSO to control end user devices from an external IP address, usually connected to the Home EMS.
- However, expensive and should not be included in retrofitting

Some heat pumps in Germany are manufactured with an SG-ready label. This label guaranteed operation in 4 states
- pump is switched off for maximum of 2 hours
- heat pump is placed in energy efficient operation, taking into account the maximal switching time of 2 hours by guaranteeing a certain level of thermal storage.
- A switching recommendation is sent to the heat pump to alter its electrical consumption pattern by modifying the setpoint of the room/thermal storage temperature
- Compulsory signal to change compressor or setpoint temperature.

However, non of these allows for user participation in the market.
## Further Readings

## Questions

- Wear and tear concerns on direct control of compressor levels
- What are the sequencing algorithms used to determine which heat pumps turn on and off. Is there an optimal way to do this. Is there a way to design economic incentives to users
	- What if the users are not home?
## Limitations

- Does not go deeply into the pool aggregation control strategy.
- Need to use a more precise Dymola model of the heat pump

https://orbit.dtu.dk/en/publications/heat-pumps-supplying-district-heating-and-ancillary-services-for-/

This is a PhD thesis, so the review will only look at a part of this paper.
## Contributions

Outlines that the flexibility of small scale heat pumps have been demonstrated in many case, large scale heat pumps does not have the same evidence. In regards to flexibility and energy efficiency.

- Investigates how large scale heat pumps can contribute to ancillary services in combination with other units.

Looks at the control structure, regulation time, and the influence of cycle design and its influence on dynamic behavior. Validated against measured data
- Investigates the cost of operating heat pumps flexibly
- Operating heat pumps (ammonia based) with faster regulation FCAS? (Such as EV batteries)

Identified problem in the suction line, and proposed solution to avoid the droplet formation in the suction line.
- Provided design recommendations for fast-regulating heat pumps

The goal is to participate in the frequency normal reserve market and deliver the regulation power within 150s
## Content

- Electric boilers can respond very quickly to signals from the electricity grid
- According to experiences from Stockholm and Gothenburg in Sweden, it is technically feasible to use large-scale heat pumps for intra-day regulation [49] [26], but the intermittent operation of heat-pumps can be constrained by mechanical wear of the components, as well as several minutes start-up time and low COP during start-up [50] 

It is most likely that a compressor part, electric motor and gear box are influenced by a more flexible operation

Provides a good summary of the ancillary market in Europe, which can be compared to Australia

![[Screenshot 2026-06-15 110445.png]]

There are further notes in the literature review about the refrigeration cycle. The purpose of a two stage heat pump is that it is able to operate at partial capacity (65%).

For the flexible control of the heat pumps, the control system must be able to react to disturbances of boundary conditions and keep the system in the desired operational state. There are $5$ variables to control
- Compressor power
- heat transfer in the condenser
- heat transfer in the evaporator
- the valve opening
- active charge in the cycle

Note that variable loads of the heat pump is enabled by a variable speed drive for the compressor and electric valves.
- Start up of the heat pump is contingent for the refrigerant falling back down into the vessels. In the base case, the heat pump can only participate in the secondary reserve market
- During startup, residual heat from the last operation causes an overshoot at the start
- Note that most primary frequency market requires ramping to full power in 30 seconds

There are various control algorithms for heat pump control

![[Screenshot 2026-06-15 120407.png]]

Each control variable is controlled by one control variable (SISO loop), and you can have multiple SISO loops, although if there are strong coupling between different SISO control loops in the system, then the transient response will take longer.

- The paper did experiments to check the transient response time of the heat pump in the base case. Simplifications are made in modelling as expected.

### Problem

To provide frequency services, the heat pump must be able to jump in the power uptake set value from the full load to different part load levels and up again
- Or operate at intermediary part load and bids s capacity of half the difference between minimum and maximum load on the reserve market.
- Regulation with the heat pump and quick-starting unit. Here the heat pump is operated at full load and may provide a maximum regulation capacity of the difference between the minimum and maximum load.
The paper did not consider the black start of the heat pump due to settling times required for the heat pump and due to frequent start-ups causing wear and tear on the system components.

As the heat pump ramps up and down, there will be a change in the saturation temperature of the low stage compressor as there is a changed outlet temperature of the heat source stream. (This change reacts faster than the wall temperature, which causes droplet formations) This will cause an increase in evaporation temperature and saturation temperature, causing sudden droplet formation that can damage the compressor.
- Note that this effect was negligible in the higher stage compressor due to the separation of the time constant.
- This presents a problem as droplet formation in the suction line during fast ramping needs to be safely avoided, but that contradicts the concept of fast ramping. The peak in the saturation temperature is also larger for larger load changes

Found that you need to preheat the suction lines with 300-400W of power, which eats into the profits.

Non-optimal control strategy can result in prolonged undershoot of the power uptake and heat flow rate.

Furthermore, another problem noted is that not all surfaces can be superheated. One way that the thesis got around this was by superheating the fluid that goes into the suction chamber of the compressor. However, this will require more energy (2kW and 7.5kW of heating, which is )
### Solution

1. Directly controlling the compressor rotational speed, so that the power uptake can be measured without delay as a change int he temperature evaporator outlet. 
- But this control algorithm was not able to ramp fast enough for the FCR-N regulation, as they need a ramping constraint on the power uptake control. There is also a risk of sudden droplet formation in all of these cases


## Questions

What happens if you don't care about the temperature set point, and just the power uptake, what would happen to the heat pump operation. It wouldn't matter for the temperature of the water since it is going to a storage unit? In that case you would be limited back how fast you can switch between different modes of the heat pump

This assumes set points in thermal outputs and thermal input sources, what would happen in more realistic scenarios?

## Limitations

- This paper only looks at frequency stability, but does not consider angular and voltage stability (most likely because voltage stability is more local phenomenon)
- In the context of district heating, most likely because it's the lowest hanging fruit
- Does not answer why e-boilers cannot be used instead
- District heating have lower temperature requirements compared to industrial applications
- Does not address aggregation
- There is no experimental validation of removing the undershoot through electric boiler compensation
## Further Readings

[52] supplying ancillary services using individual heat pump pools

Nordhavn is a Dutch precinct that acts as a living lab for various renewable technologies, including renewable thermal technology.
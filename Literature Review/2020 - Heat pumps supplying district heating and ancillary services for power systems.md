
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

To provide frequency services, the heat pump must be able to 
## Questions

## Limitations

- This paper only looks at frequency stability, but does not consider angular and voltage stability (most likely because voltage stability is more local phenomenon)
- In the context of district heating, most likely because it's the lowest hanging fruit
- Does not answer why e-boilers cannot be used instead
- District heating have lower temperature requirements compared to industrial applications
## Further Readings

[52] supplying ancillary services using individual heat pump pools

Nordhavn is a Dutch precinct that acts as a living lab for various renewable technologies, including renewable thermal technology.
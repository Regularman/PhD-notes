
https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7890446

## Overview

Used a hierarchal control framework and an aggregated Thermal Battery (TB) model to handle the heterogeneity of the inverter AC. The performance of the TB with Lithium-ion batteries are compared and it is shown that the aggregated TB model works well with the power dispatch model.

- Note that centralised (as opposed to hierarchal) loads are used to control loads to take part in demand response. However, this is not feasible with a lot of end users and privacy concerns.

Inverter AC have variable speed units in the compressor, and has higher energy efficiency. Up until that point, only fixed frequency AC has been thoroughly studied.

## Problem

Uses hierarchal control to solve the two problems of centralised aggregated control;

- Privacy concerns
- Computational burdens

Proposes a thermodynamic model of an inverter AC system $$C_a\frac{dT_i}{dt}=\frac{T_o-T_i}{R}+Q'-Q$$
as well as an electrical model for the power consumption. Since both $P$ and $Q$ is a function of the frequency of operation $$Q=\frac{k_2}{k_1}P+\frac{k_1l_2-l_1k_2}{k_1}$$
Through this model, it is possible to adjust $P$ continuously via controlling $f$ to change $T_i$.

The paper also presents a lithium ion battery model and compares it with the thermal battery in hierarchal control. There has been many models of the battery and relevant dispatch models have been developed, but not for the AC. Therefore, a TB model for the AC is developed to fit into existing dispatch models.

Outlined the performance difference with lithium ion batteries. Would be cool if there was a way to standardised this model, or have a universal model for all heat processes.

## Findings

## Limitations

Modelling an AC as a battery is not accurate as it can only act as a sink. But it's saying that the temperature can vary between $[T_{min}, T_{max}]$, with stored energy being the greatest at $T=T_{min}$. However, the air conditioning cannot supply electricity back into the grid, only shave the demand.

Each end user can set a temperature range $[T_{min}, T_{max}]$ that they prefer. What happens with various distributions of temperature ranges?

- What about the wider effects of peak shifting?
- Introduce more variables such as ambient temperature, presence of homeowners, priority stacking in aggregation step.
- The objective of the optimal dispatch is to maximise price 
## Further Works

[[2013-10- A generalised battery model of a collection of Thermostatically Controlled Loads for providing ancillary service]]


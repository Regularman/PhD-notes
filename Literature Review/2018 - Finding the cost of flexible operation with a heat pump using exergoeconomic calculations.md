https://www.sciencedirect.com/science/article/pii/S0360544218305024

## Contributions

The operation of heat pumps under ancillary services and heat demand comes at the cost of increased investment and additional losses in the conversion system. What are these losses? The paper aims to address these issues.
- The actual change to the system and
- The associated costs

This is done so in an dynamic exergoeconomic framework.

The paper also provides a way to allocate the cost between heat and demand flexibility.

The case study is a district heating system that was designed for Ocean Quay cruise ship terminal in Copenhagen.
- Water to water heat pump replaced oil burners and has a nominal capacity of $800kW$.
- The system also has a stratefied storage tank of $120m^3$ 
- 2 electric boilers $100kW$ each

Supply a constant $70\degree$C into the district heating grid.

## Content

The system was fromulated in Modelica and implemented in Dymola.

Demand data was obtained as heat loss in distribution network plus the accumulated demand of all the buildings.
- In reality, this demand would be forecasted

Included how to model heat pump operation based on COP and exergy. 

The control algorithm used ancillary market data to highlight how the heat pump system can respond to it, done using a PI controller.
- The heat pump went to full load for down regulation signal and zero-load for up regulation signal.
- In reality, you can do partial load, or aggregate the heat pumps to perform frequency services.

![[Screenshot 2026-06-17 at 12.04.29 am.png]]

Outlines how exergy streams can be used to define the flow of exergy throughout the system. Using this, they can solve for how much exergy is destroyed during ancillary operation compared to normal operation.
- This destruction of exergy is inherent 

Note that in exergoeconomic analysis, a cost is assigned to all exergy streams, which allows us to determine the cost of exergy destruction in every component.
- This allows us to look at the source of cost throughout the system and how they can be lowered

They also accounted for levelised cost stream in addition to the electricity cost and the cost stream associated with the material stream.
- Cost of electricity included historic spot market prices with tariffs included

Ultimately, the paper was able to calculate a specific cost for the provision of ancillary services, 
$$\frac{\frac{C_{heat}+C_L}{E_{heat}+E_{d,flex}-E_{d,nonflex}}\times (E_{d,flex}-E_{d,nonflex})}{\text{Joules provided to ancillary market}}$$

This specific cost can be compared to the electricity spot market to the quantify the actual benefits of providing ancillary services.

However, we need to attempt to calculate the cost without so much information, especially since we can't due do a full exergy analysis for every industry.

The study found that the specific of the heat pump in flexible operation was higher due to the higher usage of the electric boiler to heat up water from the thermal storage to satisfy demand.
- Electric boilers also had a lower exergy efficiency than heat pumps

Higher utilisation of the electric boiler and storage lead to higher exergy destruction.

The operation of the heat pump in flexible mode was 4,607 AUD/year (converted from DKK). However, does not show the revenue obtained.
## Further reading

[16] Impact of heat pumps and electric boilers and their impacts on the price of regulating powers
[32] gives annual discount rate and nominal escalation rate for operation and maintenance cost of heat pumps

## Questions

- What is the corresponding cost of providing the same ancillary services with BESS? What happens to the marginal price when thermal batteries enter the market, what will it mean for the profitability of BESS?
	- What policies or mechanisms can ensure the coexistence of both technology.
	- What happens when there's 300MW of thermal storage bidding at a low price in the ancillary market?

## Limitations

- Does not look at variation in electricity prices, which cannot truly capture the volatile spot market in the NEM today
- The problem with exergy is that you need specific number for the process and detailed process engineering understanding, which might not be available in industry.
- Did not include bidding strategies, just bidded in at whatever the price of the market gives.
- Does not allow for the possibility of an oversized heat pump and storage, and analyse the cost of this, as opposed to having electric heaters.
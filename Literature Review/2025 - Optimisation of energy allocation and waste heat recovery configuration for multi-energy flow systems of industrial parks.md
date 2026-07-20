https://pubs.acs.org/doi/10.1021/acs.iecr.5c02859

This study is concerned with how to optimise the the cost of the system whilst maximising waste heat recovery between two chemical plants. Natural gas is used to generate electricity to supply the plant, and the residual team is collected in three separate grades for heating demands. However, this means that steam is used as a heat transfer medium, which has higher heat loss and is therefore less efficient. This contrasts 5GDHC, which has a near ambient working temperature to reduce heat loss and enable anergy integration.

- Therefore, it can be said that the proposed super structure is another heating paradigm all together.
- However, can be useful to look at the different options for integrated multi-energy systems in a industrial park.
- Furthermore, the study only looks at operational optimization, rather than whole of life cycle embodied impact
- Does not use heat pumps for heating demand, rather uses an absorption heat pump

| Process                            | Input                      | Output             |
| ---------------------------------- | -------------------------- | ------------------ |
| Organic Rankine Cycle              | Low temperature waste heat | Electricity        |
| Absorption Refrigeration Cycle     | Heat                       | Cools fluid medium |
| Absorption Heat Pump               | Heat                       | Heat fluid medium  |
| Electric Compression Refrigeration | Electricity                | Cooling            |
The objective function is to optimise the energy superstructure presented to satisfy the cooling, heating, and electricity demand of the industrial park. A simplification of how the plants can be integrated is shown below.

Cooling mechanism allows one to transfer surplus cooling capacity from waste heat-rich plant to others via pipelines, for balancing cooling demands across the park. This can be achieve by creating cooling demand in waste heat rich plant (rather than using waste heat for electricity, although this behaviour will have to be optimised.)
- Centralised waste heat is used to drive the ORC, ARC, or ECR process to provide cooling capacities or electricity
- Distributed ORC, ARC, and ECR are used to process onsite waste heat, while centralised ORC, ARC, and ECR are used for the entire industrial park

![[Screenshot 2026-07-20 122139.png]]

## Optimisation model

The paper then establishes an MINLP (Mixed integer non-linear programming) to optimise the system structure and configuration. The model consists of 5 parts that are modelled

1. Intraplant heat integration: After matching hot and cold processes for heat exchange, the model identifies a cold stream that needs heating and a hot stream that needs cooling
2. Interplant heat integration: Classifies the hot and cold stream as waste heat sources and sinks. There are different grades of waste heat (high grade used to generate steam for indirect heat integration, low grade heat can drive ORC for power generation or ARC cooling production. Unusable waste heat is recovered via cooling fluid). Heat sinks are also classified by high, medium, or low grades
3. Waste heat recovery system
4. Steam power system
5. electricity balance

As well as the objective function, which minimises the cost of the interplane heat exchanger network, the cost of the waste heat recovery system, and the cost of utilities.
- Cost of heat exchanger network is just based on the fixed and area cost
- Waste heat recovery system is the equipment cost + transportation costs for the waste heat. These costs are defined in table 1.
- Showed that significant variation exists for cold pipelines under different technologies. What is the difference?

The model is solved for the intraplant model first and then the integrated design of the interplant heat exchange network. Solved using GAMS on CPU.
## Results

Analysed under two case studies. Case 1 has 8 plants and Case 2 is a 6 plant industrial park that removes two from case 1 and reduces a significant amount of waste heat and a part of the cooling demand.

Leaving heat exchange integration to the intra-plant level will leave significant amount of waste heat under-utilised, which results in energy inefficiencies.

Furthermore, different waste heat recovery configurations are proposed. 
- Optimal (cost)
- Centralised WHRC: Case two and three were configured to highlight the benefits of hybrid waste heat recovery configurations.
- Distributed WHRC
- Distributed WHRC without any cold sharing

Ultimately shows that purely centralised and purely distributed system is suboptimal within complex industrial parks. Hybrid mode saves 2-8.5% in total cost compared to using a single predefined configuration mode.

~={red}Does not look at operational variability.=~
~={red}- Need to discuss resilience! Resilience modelling is important =~
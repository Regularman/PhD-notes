https://www.frontiersin.org/journals/climate/articles/10.3389/fclim.2022.820261/full

## Contributions

Describes a methodology to incorporate technological learning curves into TEA and LCA analysis. Ultimately, this methodology is done on a $CO_2$ mineralisation case study.'

Ultimately, this is a TRL based approach.
- One of the challenges is that low TRL technologies lacks the data required to forecast the performance at large scale deployment.
- The goal is to inform investment pathways and policies around CCU technology.

Direct comparison of new technology with existing infrastructure is not 'apples for apples', because existing infrastructure already have the benefit of learning period and technological experience. 
- All existing literature circumnavigates this by assessing data for similar 

The paper proposes using granular learning curves and also projecting GHG emissions predictions (current studies focus on costs).
- The disaggregation of the technology into each of its components allow for more informed predictions of cost decrease moving forwards.

The paper uses OFLCs to model how capital cost and GHG emissions could change with increased deployment 

## Content

Note that learning rates for different metrics of the same technology (cost, GHG emissions, efficiency), may be different. The factors that contribute to improved learning are
- labour efficiencies
- standardised manufacturing
- optimization of product design

However, it should be noted that there are exogenous factors that affect costs, such as fluctuation in labor and energy costs, in addition to endogenous learning factors. These exogenous factors can create biased results when analysing past data. 
#### One Factor Learning Curves (OFLC)

OFLC looks at the aggregation of all contributions to technological readiness into one factor. This leverages accessible data such as investment costs or production volumes. However, this can only be used for technologies that have reached a certain level of commercialisation, as cost data are generally non existent or confidential at early TRLs. $$c_t = c_o (\frac{P_t}{P_0})^{-\alpha}$$
Learning rate (LR) is described as the percentage cost reduction with each doubling of cumulative production capacity. $$LR=1-2^{-\alpha}$$
#### Two Factor Learning Curves (TFLC)

TFLC disaggregates the learning factors into learning-by-searching and learning-by-doing. This allows integrating a research variable that helps with modelling early stage technologies. $$c_t=c_0(\frac{P_t}{P_0})^{-\alpha}\times(KS)^{-\beta}$$
#### Multi-factor Learning Curves (MFLC)

In MFLC, learning by doing is disaggregated into learning by using, learning by interacting, and learning by learning by deployment to integrate the effect of user feedback on the learnign curve

#### Comparison with similar technologies

CCU can be compared to CCS due to capture components of both technologies, but performance changes with each individual capture technology.
- A report from NETL analysed the learning rates for estimating costs between FOAK and NOAK plants.
#### Recommendations

1. Understand technology at the component and product level to understand the drivers of learning
2. Include technical, economic, and environmental learning models
3. Combining projections from experts with extrapolated performance metrics generated with learning curves
4. Considering LBS effects using patent and experimental data when possible
5. Prioritise use of historical data and literature values over rates from similar technologies
6. Need to acknowledge the uncertainty within the data. These uncertainties can be mitigated through sensitivity analysis
## Further Readings

Papers on energy generation and storage for calculation of learning rates
- Elia et al 2020
- Thomassen et al 2020

Look at NTEL paper
## Limitations

Rather than looking at the performance improvements of a technology class, this study looks at learning improvements of a design from FOAK to NOAK.
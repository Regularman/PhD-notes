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

#### Methodology

This is informed by the 2005 IEAGHG report, which states that the technological readiness level of 
1. Break each plant into its technology subsection
2. Estimate the current plant costs and contributions of each subsection
3. Select an appropriate learning rate for each subsection/component
4. Estimate the current capacity of major plant components
5. Set the start of learning (FOAK) and ending period (NOAK)
6. Perform sensitivity analysis

The study uses the formula $$\alpha =\frac{\log{(1-LR)}}{\log{(2)}}$$
The LR is based on historical LR from other similar technology, using data classification methodology from [[Thommassen 2020]]. In this study, the assumption for leanring rates comes from literature about CCS technologies. Subsequently, as learning rates are normally defined for CAPEX rather than OPEX, the EPC is found as $$c_{EPC}= TDC*(1+c_{indirect})$$where the TDC is total direct cost and $c_{indirect}$ is the indirect cost of the plant. Then the process and project contingencies must be added $$TPC_{FOAK}=c_{EPC}*(1+c_{process}+c_{project})$$We can then use the learning index $\alpha$ and $N$ , the number of plants necessary to reach the desired NOAK plant $$TPC_{NOAK}=TPC_{FOAK}*N^{-\alpha}$$
The number for $N$ can be determined via several methods
- Calculating the cumulative capacity that would need to be installed for a plant to break even
- Finding the cumulative capacity where the learning curve flattens out
- Using a number of plants that would translate into pre-defined market share
- Using a number of plants that correspond to those that would receive external subsidies. ~={green}For example, in this study, they assume that up to 5% of cement plants in Western Europe will receive public subsidy, translating to around 10 plants at the NOAK level.=~

Alternatively, a more granular approach will be to estimate cost learning for each component, and then have a composite learning rate known as $$LR_{composite}=\sum_i[LR_{sys, element}*\frac{TDC_{sys,element}*(1+c_{indirect})*(1+c_{process}+c_{project})}{TPC_{overall,sys}}]$$
For emissions, a separate methodology can be followed, with a new learning index and learning rate used for the metric. For example, in this study, an emission floor was calculated using $2$ proxy factor, the recycling of additives (the amount of $CO_2$ recycled back into calcium carbonate is limited and process yield cannot exceed 100%). An environmental learning rate of 4.35% was assumed based on average learning rates for operating and maintenance costs for post-combustion $CO_2$ capture facilities.
- However, there should be a theoretical limit on how much the ~={red}foreground system=~ can decarbonise. Any factors after reaching this theoretical limit needs to come from exogenous systems under considerations such as lower scope 2 emissions.
![[Screenshot 2026-11-02 at 10.00.47 pm.png]]
![[Screenshot 2026-11-02 at 10.00.57 pm.png]]
![[Screenshot 2026-11-02 at 10.01.06 pm.png]]
![[Screenshot 2026-11-02 at 10.01.26 pm.png]]
#### Results

Finally, the learning rates for each component of the technology can be estimated based on the TRL level
![[Screenshot 2026-11-02 at 10.02.52 pm.png]]
## Further Readings

Papers on energy generation and storage for calculation of learning rates
- Elia et al 2020
- Thomassen et al 2020

Look at NTEL paper (2013)

Reuben 2019 and Roussanaly et al 2013 provides a hybrid bottom-up/engineering economic and a top-down/learning curve approach for cost estimation.
- The early FOAK stage has additional redundancy to reduce risk of failure during operation. These designs are optimised in mature technologies.
- However, NOAK plants should not be derived using a bottom-up costing approach as it is not really possible to odel high-level cost of future plants
## Limitations

Rather than looking at the performance improvements of a technology class, this study looks at learning improvements of a design from FOAK to NOAK.

The limitation of the learning curve, also mentioned in the NTEL report, is that learning curves does not account for the cost increase that can occur during the start of a project's development
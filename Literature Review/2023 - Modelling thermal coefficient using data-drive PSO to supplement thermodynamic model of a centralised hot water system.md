## Contribution 

Uses a mechanistic model and particle swarm optimisation (This is used to optimise the parameters in real time to improve the accuracy of the model) to visualise thermal behaviour and energy flow of district heating system. This connects the heat network, the heat users, and the exchange stations, with the variables being 
- Heat load
- pipe characteristics and,
- heat transfer coefficient

The thermal network modelled is a centralised district heating model with a primary and secondary heating network.
- Heat is dissipated to the room using radiators.
- Heat exchangers are used in the heat substation as an interface between the primary and secondary substation

The main contribution is the prediction of the thermal exchange coefficients of the heat exchanger to improve modelling of the hot water temperature.
## Content

Where mechanistic model is useful for replicable and explainable modelling, it does not perform well with non linearity. 
- Data driven approaches can capture the internal working of the system but has weak scientific and explanatory significance

### Mechanistic model

#### Heat Exchanger

Heat consumer in the primary network and a heat source in the secondary network.
- Assumes known mass flows and heat coefficients
- Assumes adiabatic and heat conduction along the flow of the heat transfer surface can be neglected

Particle swarm optimisation algorithm is used to optimise the heating coefficients of the model in real time, this is as the heating coefficient of the heat exchangers changes with temperature, and must be calculated iteratively.
- Note that using this optimised model to estimate the thermal coefficient of the heat exchanger, the data was able to achieve a more accurate representation of the hot water temperature given all of the inputs

Note that the heat substations uses heat exchangers rather than heat pumps.

### Piping network

Disregard the branching and merging of piping network and supply and return piping are single segments

Neglect radial direction of the pipe walls.

The net heat stored in the piping network is equal to the heat input from the hot water minus the heat loss due to heat dissipation.

## Model for the users

- All households assumed to be in a virtual room
- Surface temperature of the radiator is an an average of the supply and return temperature 

## PSO Methdology

The data driven approach takes the data distribution of the heat coefficients to be a mixture of Gaussian models, using an expectation maximisation formula to maximise the posterior probability that the data is in the distribution through an iterative process until the results converge.

The Bayesian Information Criterion is used to ensure that the optimal number of clusters is used in clustering analysis.

PSO is a ppulation based search algorithm inspired by the behaviour of bird flocks.
- Starts by initialising a group of individuals in a search space, where each particle represents a candidate solution
- Uses a fitness function to continuously update their position, and the particles converge towards an optimal solution (This might be the mean error between the return water temperature using operational data from a heat exchange station in Dalian in 2022 to 2023)
## Question

1. The thermal model is not explained properly, the equations are messed up, so will need to look into my own thermal model development.
## Limitations

## Further Reading
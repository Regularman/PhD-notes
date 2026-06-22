# 1-06-2026 - First day meeting 

Attendees: Robert Taylor, Melvin Chan
## Content

The Iberdrola project will have gaps in module B for looking into the decarbonisation options and supply options from the tool. The inputs will be the product of the process and the energy bills of the factory. 

Sami requires a thorough plan and methodology before we start. 

For everything that I look into, try to be able to publish something from it.
- Have a look into each of the three stakeholders (DNSP, consumer, and Iberdrola). Structure PhD such that each of the stakeholder is included
- Sami is life-cycle assessment focused. Having a look at the whole of project impact on the grid and how that will impact carbon savings 

# 3-06-2026 - Weekly meetings

Attendees: Thesis group, supervisors, Melvin
## Prep and questions

## Content

Build more on what Tom was doing

Look at typical operating profile

Impact reduction potential is limited to electrification for heat as a service, depending what happens at the end of the lifecycle.

- Circulation of equipment in the heat as a service
- Material consumption reduction from centralised
- how are they quantifying and how are they selling it
- focus on the relevant technologies and where are they manufactured and what the lead times are

# 10-06-2026 - Weekly thesis meetings

Attendees: Thesis group, supervisors, Melvin
## Prep and questions

Onsite energy supply options for module 2, implementing storage. 
- Outline how it will interact with the spot market and ancillary market for different supply options

Need to obtain git-hub codebase for Tom Shepherd's optimisation code first.

Interested to understand impact on aluminum refinery scaling up, does the upscale in operation provide additional opportunities for decarbonisation. 
- This is due to dwindling copper supply will see switchboards switch to aluminum based
## Content

Anchala needs to understand how the data needs to be formatted.

Rohan will do supply options and how that will replace. 

Build on Tom's codebase and think about feasibility study. 

- Figure out the ones that Daniel and I need to do

# 12-06-2026 - Meeting with John and Rob - PhD kickoff

## Prep and Questions

- look at the operation of heat pumps under different operational strategies
## Content

John is interested in co-supervising, add him to GRIS as the next step
- John's scope will be to help advise methodology for looking at heat pumps and whether there are any analytical technique to help with that

Think about the next step in the technological ladder, is there anything we can add to a heat pump such that it can respond to the faster response ancillary market
- How can test and implement these machineries/new design features? 

look at lifecycle impacts of heat pumps under cost optimal and carbon optimal strategies. 

Firm up scope AND methodology for Iberdrola

# 15-06-2026 - Weekly meeting with Rob

## Prep and questions

- Starting point for foreign collaboration
- Should I be doing any courses, and does my PhD cover the funds

### Plan
- Hardware in the loop? This will allow use to see market impact and for faster frequency responses and it will not rely on fully modelled dynamics. 
- I want to get to a high level tool for technology mix
- Need to start making the methodology
- Looking at heat pump control will also be interesting
- VPP heat pumps as a baseload to provide inertia under FPP scheme
### What I have done

- Read a lot papers does techno-economic modelling of heat pumps, one for heat-pump plus solar thermal. Copied down what they did and how they did it, a lot of LP optimization for the heat pump and sensitivities. Gaps in partial load operation and industrial applications of larger heat pumps.
- High level summary on circular economy in Europe (development of takeback systems, implementation of digital passport)
- Started power systems course
- Spend 20 minutes at the start of the day reading articles on market analysis in the NEM. Recently been looking at the characteristics of the FCAS markets in the NEM (talk about the impacts of semi-scheduled assets)
- Got in contact with Tom

## Notes

The 3 topics/buckets that my PhD will fall into

1. Looking at business case at each scenario/percentage of electrification. It would be good to understand the value prop for each technology under the EPC and HaaS business models. it would then move into the calculation of revenue and green house gas emissions, and finally in the last stage, the future scenarios such as rapid battery uptakes

![[topic - 1.png]]

2. Lifecycle assessment, looking at the value chain under HaaS. Need to confirm with Sami about the actual research question
3. Technology option. For example, looking at hardware in the loop for control algorithms, or adding a flywheel to the heat pump in experiments and testing the frequency response.

Look at audits for UNSW course, free and don't need to do assignment

Would be cool to pursue one day a week at Iberdrola, next time we meet with them, prepare a list of things that I can do in their office and the value that I bring.

For the RACE project, focus more on collaborating with Amr and coming up with techniques and frameworks that the thesis students can follow

# Quick meeting with Amr

There are three options for the replacement of gas boilers. Currently, they give the name plate capacities of their equipment, energy bills, and utilization. We just don't know how long each equipment is used for

- We know how much gas they use, and therefore can use that as a basis for the sizing of the heat pump/electrification technologies to investigate potential GHG and cost savings
- They want to electrify a certain gas boiler, in which case we can get their nameplate capacity and see how they 
- They might want to electrify a certain process, in which case we need the gas distribution for each process through the EFA

Adding seasonal load profiles as well

Below is the general approach to get the economic analysis

![[Screenshot 2026-06-17 142134.png]]

# Github Codebase meeting 18/06

### Meeting with Rohan, Anchala, and Amr to firm up what to do for codebase

Rohan is doing the supply options, compiling the technology COPs to see how it impacts emission factors.

Anchala's goal is to figure out how to use the Sankey diagrams

Iberdrola is only worried about the use phase carbon emissions. 
- Amr has calculated the Global Warming Potential of each technology in each state based on the grid 
- The problem is that is doesn't consider the coupling of technology
- Furthermore, it misses the opportunity cost of electrification and voltage regulation at the distribution level
# Weekly PhD meeting 22/06

Attendees: Amr and Rob 

Presented the HaaS lever presentation to Rob and Amr. They were happy with the risk framework around identifying the value chain and risks acceptable within Iberdrola's risk tolerance. The next step would be to
~={red}- identify and quantify the risk through Monte Carlo analysis (as an example)=~
~={red}- interesting to set up market research interviews with Antora or Johnson's Control or ClimaTech to learn more about their business model. Some questions to ask might be =~
~={red}	- Why everyone does the finance+D&C+maintenance part of the HaaS contract=~
~={red}	- Why do they insulate themselves from the energy procurement risk=~
~={red}- Apply risk framework to specific technologies, currently risk agnostic.=~
~={red}- Find more case studies (>50) and do a heat map of value chain against risk values (this would be after quantification)=~
~={red}- Look at Eurosun for Viessmann ancillary services=~

Another example is Qantas with general Electric who owns their engines which can be looked into.

There is a report due in September, HaaS information can take up a page or 2 of this. Also there will be a meeting with Iberdrola this term with all the thesis students, they can be informed on this.
- My work will mostly be integrated with Module 4

RACE was not able to award the top up as they are no longer accepting any more PhD students.

~={red}- Look at A2EP refrigerant reading materials for heat pumps=~
~={red}- It would be cool to reach out to IRG and industry bodies before teh September reports to inform them of the results of the decarb tool=~
~={red}- The Iberdrola meeting will be Anchala and Rohan and Ali and then demonstration of the decarb tool.=~

In the aspect of stress testing, find the breakeven price point for batteries to be competitive in the market. What happens as battery gets cheaper, can it compete in bidding with thermal batteries.

With Sami, take notes of what he says and questions he asks, and in the next meeting, answer those questions/queries.

## Meeting with Sami

### Prep and Questions

- Auditing GSOE9340
- Show him the possible research questions
- Explored some take-back schemes and reverse logistics in the context of a heat as a service system where the ESCO (Iberdrola), will take on several roles in the value chains. What kind of dynamics and opportunities will that open up
	- Talked about that fitting in with Module 4 of the wider Iberdrola project
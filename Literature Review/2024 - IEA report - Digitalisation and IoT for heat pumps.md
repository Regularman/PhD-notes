
https://heatpumpingtechnologies.org/publications/annex-56-digitalization-and-iot-for-heat-pumps-final-report/

Task 1: https://heatpumpingtechnologies.org/publications/annex-56-digitalization-andiot-for-heat-pumpstask-1-state-of-the-art/


## Contributions

Provides a structured overview of IoT enabled heat pumps and commercial products and services. Includes 44 applications examples as well as the opinion of experts from Austria, Denmark, France, Germany, Norway, Sweden, and Switzerland

- Heat pump operation optimisation and comparison with other heat pumps
- Predictive maintenance
- Heat pump operation commissioning: ensuring that the heat pump is sized appropriately and minimise energy consumption from the outset
- Provision of flexibility and HaaS
- Fault detection
- Control

In some of the Deep Dive sessions, the expert seminar built on HIL and digital twins as development for IoT of heat pumps.

## Content

Data exchange and use allows for better provision of flexibility. One of the challenges that was found in this activity is that interoperability between heat pumps of different manufacturers and different actors in the energy system is a key barrier in balancing generation and consumption.

Connected heat pumps will play an important role in maintaining grid security. The paper propose that a European data space for the exchange and use of energy data, as well as a code of conduct for ~={orange}interoperability=~, will enable more devices to participate in demand response and increase the cyber security and resilience of the system.
- ~={orange}Data security and protection=~ is a major barrier to the adoption of digital technology in the residential area. Conversely, in industrial applications, IoT platforms and cloud computing are used for monitoring in manufacturing, cross-site energy management, and control of centralised plants.
These considerations are in addition to the ~={orange}cost=~ consideration inherent in digitalization of assets. These are the risks of digitalisation, although it has a potential to reduce $350 Mt$ $CO_2$ by 2050 due to demand management and smart controls.

Note that the global IoT market is worth $457 billion in 2020, with smart cities being 26% and Industrial IoT with 24%, smart buildings is 14%.

### State of the art - Topics of interest

~={orange}Industry 4.0=~ represents movement from automated assembly lines to cyber physical systems that can address the flexible demands of modern day manufacturing $\rightarrow$ This will lead to ~={orange}Industry 5.0=~, a fully digital ecosystem with machine 2 machine communication (IoT).
- The Internet of Things is a general framework where machines can independently communicate with each other (the digital shadow of other devices) seamlessly to minimize waste and enhance efficiency in the manufacturing process. 
- The collection and processing of high quality data enables preventative maintenance and optimised operation where ~={orange}prioritisation=~, ~={orange}synchronisation=~, and ~={orange}scheduling =~are optimal.

The Industrial Internet Reference Architecture looks at various view points
- Business viewpoint, looks at IoT devices in a business and regulatory context
- Usage viewpoint, represents how IoT devices are to be operated as a sequence of activities
- Functional viewpoint, what are the functional components of the IoT device
- Implementation viewpoint, what is the technology needed to implement

Communication protocol stack. TCP/IP protocol. These protocols are relevant in how data is transmitted to and from end devices to the central cloud storage. ~={orange}However, the innovation in this PhD is not of communication protocols, and we can look mask over this complexity through simple data transfer.=~

In HIL applications, middleware such as ~={green}Fiware=~ can be used to enable communications between real systems, virtual models, and integrated services like Fault Detections.

Furthermore, there is already an existing framework to consider the digitalisation and smart energy solutions of heat pumps, known as the ~={green}Smart Energy Operating System=~. The system has embedded controllers for handling ancillary service problems and include all layers of computing including ~={orange}cloud, fog, and edge computing=~ near the IoT devices.

| Layer                 | Description                                                                                                                                                                                                                                                                                                                                                             |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Application layer     | The applications built on the internet (HTTP protocol) enables stateless text-based request response communication between clients and a server                                                                                                                                                                                                                         |
| Transport layer       | Provide transparent host-to-host communication services towards the application layer, masking the complexity of networking. TCP/IP protocol or User Datagram Protocol (UDP) are popular and guarantees reliability, flow control, congestion avoidance. The latter is the preferred candidate for IIoT as it is good for the transfer of small packets of information. |
| Internet Layer        | IEEE802.3 - ethernet connection and IEEE802.11 (family of Wi-FI standards). The Internet Protocol (IP) allows internetwork and the efficient and robust routing of data packages across the data network.                                                                                                                                                               |
| Host to network layer |                                                                                                                                                                                                                                                                                                                                                                         |
Information security is hosted on 3 premises 
- Confidentiality: access rights
- Integrity: unmodified data
- Availability: can be accessed when needed

There needs to be a negotiation of contractual agreement between data controller and processor, with standard contractual clauses approved by the European Commission being available, oh data protection obligations, e.g.
- Right to access to stored personal data
- Right to rectify inaccurate personal data
- Right to data portability
- Right to restrict the processing of personal data
### Data analysis techniques 

### Business Models
## Limitations

## Questions

Digitalisation in Australia? Look at DER roadmaps, subsidies for smart metering.

Is there an IEA report on heat pump flexibility and grid services?

How do most ESCOs provide maintenance services? Do they subcontract the digital monitoring capability?

What is a heat pump with magnetocaloric (bottom cycle) and vapor compression (top cycle), and why is it special.
## Further readings

Fact sheets provides in [https://heatpumpingtechnologies.org/project56/factsheets/]

[3] 1/3 of R&D projects for IoT in europe addresses Smart City, Smart Energy, and Smart Building applicatons.

Look at ARENA project with data exchange in DER roadmap

Check out the Deep Dive Session highlighted in the document.

Look at HP-COM for report on ICT of heat pumps.  https://www.teknologisk.dk/projekter/projekt-hpcom/37449 




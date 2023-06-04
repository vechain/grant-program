# VeChain General Grant Application Template

## Project Overview

- Project: Upgrade and Deployment of public Nodes
- Team Name: favo
- Payment Address: `0xcC4B3412161Ea88d0538D2Da15cffa74af0eE9D4`

### Overview

Since June 2022 the VeChainThor public node, node.vechain.energy, has been available for use by the VeChain community. It is one of only a handful of public VeChainThor nodes that are operational on the network. It is used by several community applications as either the primary or fallback node. I am seeking a grant to upgrade the hardware of the existing node, to deploy an additional public VeChainThor node and to create and deploy a virtual proxy node.

The hardware of the existing node, node.vechain.energy, is on the lower end of the recommended specifications and with increasing usage a hardware upgrade would ensure better performance. Adding an additional second node will increase the overall number of available public VeChainThor nodes. This second node will be located in a different region than the first node, offering lower latency for users in other areas of the world. The first node is located in Germany, a second node will be setup in the USA.

Additionally a virtual proxy node will be created and deployed to increase network resilience by providing a fixed entry point that leverages all existing public nodes. Similar to a load balancer it can automatically redirect requests to live nodes only and at the same time ensure that failed requests are retried.

The grant will be used to setup upgrades and cover the costs for two years. In the meantime it will provide a reliable solution for community developers and projects.


## Project Details

### 2x Servers

At the moment one public server exists at https://node.vechain.energy. It is a dedicated server at the lower end of the recommended hardware configuration.

The existing Node #1 will receive an upgrade close to the recommended hardware configuration. The location is Berlin/Germany.

An additional server will be setup in a different location in Las Vegas/USA.  

Both servers will be made accessible:

1. Directly with HTTP/HTTPS
2. DNS weighted entries in AWS Route53 with a Geolocation policy

A MainNet setup will be done only, no TestNet servers will be setup.

The specifications will be:

- Intel Xeon, 8 Core 2.6GHz 
- 64 GB RAM
- 1TB SSD Raid 1 (2x 1TB NVMe)


### Node-Rotation

As additional solution a third "virtual" node will be setup that proxies incoming requests to a list of publicly known nodes existing in the whole ecosystem.
  
If a node fails, automatic failover happens to the next one in the list, retrying the same request with another node. This creates an always-on-experience for client applications.

- if a node is unavailable, another node is tried until a node becomes available or the list of nodes is exhausted
- the list of nodes will be shared on a public endpoint
- rotation will be provided for TestNet and MainNet
- with WebSocket and HTTPS Support 

A prototype is already available at:

- https://node-testnet.vechain.energy
- https://node-mainnet.vechain.energy


### Maintenance

As a monthly average a maintenance time of 3 hours per month for the dedicated servers and 2 hours for the rotation are estimated. This includes server updates, software updates and modifications, fixes or required adjustments to keep it fully functional. Other improvements  will be made outside of the grants scope after the initial deployment.

An external service will be setup to monitor all endpoints. A public status page with the availability history and notification on outages will be made publicly available.


### Ecosystem Fit

Right now the list of nodes is so short that an outage will impact the regular community builders enormously. It is important for regular developers and projects that utilize public nodes are available at all times and that alternatives exists. Adding two public nodes and a proxy with rotation will improve the situation, increase the networks resilience and reduce dependency on individual parties.

## Team 

### Team members

- I am a fulltime IT-professional with 24 years’ experience with a focus on web and mobile applications. I am happy to share more details by email (instead of publishing it on GitHub).

### Team Website

- https://vechain.energy

### Roadmap

#### Overview

I am seeking a grant of $26,648 to achieve the following roadmap.

|  | Dedicated Server | Rotational-Node | Maintenance | Additional Costs | Total
| - | - | - | - | - | - | 
| Estimated Duration | 5d | 5d | 730d | 0d | 740d
| Full-time equivalent (FTE) | 1 | 1 | 1 | 1 | 1
| Cost (up to $30,000) | $4,000 | $4,000 | $12,000 | $6,648 | $26,648


#### Dedicated Servers

| Number | Deliverable | Specification |
|-|-|-|
| 1.1 | Node #1 | Link to MainNet Node in DE
| 1.2 | Node #2 | Link to MainNet Node in USA
| 1.3 | Route 53 | Link to DNS Entry that does Geolocation-Weighting for node #1 and #2

This milestone includes all actions related to setting up the dedicated servers:

- Order & Setup of the Operating System
- Installation of VeChainThor-Nodes
- Synchronization of the Blockchain and testing the setup
- Configuration and testing of the Webserver
- Configuration and testing of AWS Route 53

The duration of this process for two servers is estimated to roughly a weeks work (40hrs).  
The deliverables will be the final availability of the two resulting nodes the geo-weighted DNS.

#### Node Rotation

| Number | Deliverable | Specification |
|-|-|-|
| 2.0 | Proxy | Unit-Tests for functionality with outage-detection |
| 2.1 | TestNet | Link to TestNet Endpoint that acts as a node proxying all requests to a list of TestNet Nodes |
| 2.2 | MainNet | Link to MainNet Endpoint that acts as a node proxying all requests to a list of MainNet Nodes |

This milestone includes the development, testing and deployment of the functionality.  
Deployed working endpoints will serve as deliverable for both networks and unit tests that display how it works.  
The duration of the development, deployment and testing is estimated to be one week of work.


### Maintenance for 24 Months

| Number | Deliverable | Specification |
|-|-|-|
| 3.1 | Dedicated Nodes | 24 months of 3 hours maintenance
| 3.2 | Virtual Node | 24 months of 2 hours maintenance
| 3.3 | Status-Page | Status-Page with historical performance for each endpoint

Maintenance is an average number of hours to make sure software is kept up-to-date, manage potential problems, provide support if something happens or mitigate potential attacks.
From past experience it is estimate that at an average of about an hour weekly can manage all four setups (2x dedicated + 2x virtual). While some weeks might have zero required work, a single event can require up to a days work resulting in an average of one hour per week.


### Additional costs

The following are a list of additional costs that will occur during 24 months:

- Monthly Costs of both nodes are planned to be $120 per month. Over a period of 24 months by 2 Servers this equals $5,760.
- Route 53 Health-Checks are $2 per month. Over a period of 24 months by 2 Servers this equals $48.
- Route 53 requests are free for less than 1 billion requests, if requests exceed this I will cover the cost.
- The cost for CloudFlare’s paid plan is $5 per month. Over period of 24 months this equals a total of $120.
- The cost for requests are estimated to be between $5 to $50 per month, an average of $30 is used. Over a period of 24 months this equals a total of $720.

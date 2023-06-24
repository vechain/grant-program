# VeChain General Grant Application Template

## Project Overview

- Project: VeBlocks infrastructure upgrade 
- Team Name: MiRei - I am happy to provide a detailed resumee via email but not happy to have it on github.
- Payment Address: 0xcb0c81cf6742c2ea97cec01f95c08d22045edbfc USDT (ERC 20)

### Overview

VeBlocks is a community project created and managed by MiRei in October 2019 (https://twitter.com/MiRei83_/status/1186632017544388608). It is focused around the blockchain infrastructure of the VeChain blockchain (Mainnet, Testnet, etc.). Since then, Veblocks not only aggregates and visualizes blockchain statistics via https://visuals.veblocks.net, it also provides free, public and unrestricted access to full-archive-nodes of the Vechain blockchains via https://nodes.veblocks.net. 

The idea is to have a "ready-to-go" solution and lower the threshold and initial cost for new developers. This benefits every developer building on Vechain blockchain and removes all hardware-limitations to get started.


This grant is meant to further improve the reliability and response-time of the public backend and also ensure constant maintaining through the next 12/24 months. It also ensures the continuance and development of https://visuals.veblocks.net.

<br/>
<br/>

## Project Details

### VeBlocks backend

As mentioned in the overview, the basic functionality to access the vechain blockchain is already adapted. Hosting a public VeChain node requires powerful hardware. Fast responding nodes are achieved via virtualisation on a dedicated bare-metal server with the newest generation of CPUs and NVMe SSDs. At the moment, only one of these bare-metal servers is active to reduce running cost.
To provide high-availability, load-balancing and clustering of the backend infrastructure additional bare-metal server in different locations are needed.

In the final stage, the backend should consist of:
- Two dedicated bare-metal server in two different data-centers
- Each endpoint to have HTTP and HTTPS capabilities and load-balance between at least two nodes
- Access through two global CDN (Cloudflare, Azure)
- A maintenance- and continuanceplan for 12/24 months

This kind of setup requires constant care and support, so a certain amount of time is needed per month to keep the nodes running. Since 2019 I figured that about 1.5 hours per month per server is sufficient.

The goal is to provide a robust, constant, long-term solution.

### Ecosystem Fit

To my knowledge, there is no other project that provides public access to the VeChain blockchain. 
VeBlocks is already used by several applications, including 

- the backend for https://visuals.veblocks.net
- the default gateway for Sync2
- the default gateway for https://insight.vecha.in
- the default gateway for https://explore.veblocks.net
- an optional gateway for Sync
- a sync-node for https://www.vechainstats.com
- the first choice for many developers bulding on VeChain

<br/>
<br/>

## Team 

The team consists of:
- MiRei: I am a fulltime IT-professional for 15 years with focus on IT-infrastructures and IT-security. Because of an enormous amount of work, my focus has shifted away from the veblocks project in the recent weeks. With this grant I will be able to reevaluate these priorities.


### Team Website

- https://visuals.veblocks.net
- https://nodes.veblocks.net

### Team Code Repo
- https://github.com/mirei83/

<br/>
<br/>

### Roadmap

#### Overview


|  | Milestone 1 | Milestone 2 | Milestone 3 |Total |
| - | - | - | - | - |
| Estimated Duration | 30 d | 365 d | 365 d | 760 d |
| Full-time equivalent (FTE) | 3 | 1,5 | 1,75 | 6,25 |
| Cost (up to $ 30,000) | $ 2,340 | $ 5,730 | $ 6,520 | $14,590 |

<br/>
<br/>

#### Milestone 1 — VeBlocks backend upgrade

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| Expansion | Renting additional Server in different datacenters |
| 0b. | Installation | Servers will be installed/configured with the needed software |
| 0c. | Configuration | Redundant VeChain nodes will be set up on all locations |
| 1 | Clustering | After all locations are online, the locations will be clustered together to provide higher uptime |
| 2 | Testing | When the backend is in operating mode, an in tensive testing periode will be done |
| 3 | Go-Live | When testing was successful, the backend will be online for public usage |

<br/>
<br/>

#### Milestone 2 — Uptime, maintenance and improvements for 12 months

| Number | Deliverable | Specification |
|-|-|-|
| 0| monthly cost | This includes all human resources and data-center facilities for the first 12 months |

<br/>
<br/>

#### Milestone 3 — Uptime, maintenance and improvements for an additional 12 months

| Number | Deliverable | Specification |
|-|-|-|
| 0| monthly cost | This includes all human resources and data-center facilities for an additional 12 months |

Caused by higher data-center facilitiy cost and more users needing support, the 3rd milestone had to be slightly adjusted (as shown in the overview table above).


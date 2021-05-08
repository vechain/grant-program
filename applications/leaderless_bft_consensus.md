# VeChain grant research proposal template

## Leaderless Byzantine Fault Tolerant Consensus

## Applicants

Fangyu Gai (corresponding applicant). He is currently a third-year Ph.D. student at School of Engineering, University of British Columbia, supervised by [Dr. Chen Feng](https://people.ok.ubc.ca/cfeng01/index.html), who is the co-cluster lead of [Blockchain@UBC](https://blockchain.ubc.ca/). His research interests lie in distributed systems, especially blockchain systems. Most recently, He has been focusing on building efficient and high-performance permissioned blockchain databases at [Alibaba DAMO Academy](https://damo.alibaba.com/) as a research intern. More information including his CV can be found at his [website](https://fangyugai.me/).

Jianyu Niu. He is currently a fourth-year Ph.D student at School of Engineering, University of British Columbia, also supervised by Dr. Chen Feng. His research interests focus on incentive and consensus protocol designs on blockchains. His CV can be found [here](https://fangyugai.me/files/JiangyuNiu_CV.pdf).

Chen Feng. He is an assistant professor and Tier-2 principal’s research chair in Blockchain in the University of British Columbia and he is also the co-cluster lead of [Blockchain@UBC](https://blockchain.ubc.ca/). His research interests include information and coding theory, wireless communications and networking, cloud computing and big data, and very recently blockchain technology. In particular, he is interested in adapting new ideas and tools from information theory, coding theory, stochastic processes, and optimization to design better communication networks with a particular emphasis on quantum communications and blockchain technology. The primary goal of his research is to bridge the gap between theoretical advances and system implementations. For more information about him (including his CV), please visit his [website](https://people.ok.ubc.ca/cfeng01/index.html).

## Payment Address

USDT: 0x955bcFf3a3a8998C1d732C609BF2Ff22A8803a3B

## Summary

Byzantine fault tolerant (BFT) consensus has recently gained much attention because of its intriguing connection with blockchains. Several state-of-the-art BFT consensus protocols have been proposed in the age of blockchains such as Tendermint, Pala, Streamlet, HotStuff and Fast-HotStuff. These protocols are all leader-based (i.e., protocols run in a series of views, and each view has a delegated node called the leader to coordinate all consensus decisions). To make progress, leader-based BFT protocols usually rely on view synchronization, which is an ad-hoc way of rotating leaders and synchronizing nodes to the same view with the leader for enough overlap time. However, many studies and system implementations show that existing methods of view synchronization are complicated and bug-prone. In this paper, we aim to design a leaderless Byzantine fault tolerant (LBFT) protocol, in which nodes simply compete to propose blocks (containing a batch of clients' requests) without the need of explicit coordination through view synchronization. LBFT also enjoys several other desirable features emphasized recently by the research community, such as the chain structure, pipelining techniques, and advanced cryptography.

### Main field of research

Blockchain consensus mechanisms; Blockchain security / privacy

### Keywords

Byzantine fault-tolerant, blockchain consensus

## Research proposal (main body)

We have written a draft of our proposal in latex which is more scientific-friendly than markdown. Please refer this [technical report](https://fangyugai.me/files/Leaderless_Byzantine_fault_tolerant_consensus.pdf) for the proposal. Many thanks.

We believe that our work has a lot of potentials of being applied on VeChain's PoA 2.0 to improve its finality. Therefore, the purpose of applying for the grant is to continue working on this project as it is still in a very early stage.

The technical report already covers the most of the technical details. In this project, we plan to improve it in the following three stages:
1. Write a scientific paper based on the technical report, potentially working with the Vechain research team to make it more friendly to Vechain's ecosystem.
2. Implement a proof-of-concept of our proposed protocol and compare it with other related work (e.g., Casper) in terms of performance and other properties.
3. Consider to apply it into Vechain's ecosystem.

### Milestones

#### Overview

|  | Milestone 1 | Milestone 2 |  Milestone 3 | Total |
| - | - |- | - | - |
| Estimated Duration | 30 d | 30 d | 30 d | 90 d |
| Full-time equivalent (FTE) | 0.5 | 0.5 | 0.5 | 1.5 |
| Cost (up to $ 30,000) | $ 10,000 | $ 10,000 | $ 10,000 | $30,000 |

#### Milestone 1 — Scientific paper

| Number | Deliverable | Specification |
|-|-|-|
| 0 | Techinical Report | We will improve the technical report that we have been writing and make sure it is well-written and technically correct |

#### Milestone 2  —  Prototype
| Number | Deliverable | Specification |
|-|-|-|
| 0 | Prototype | We will build a prototype of our protocol using Golang for proof-of-concept |

#### Milestone 3  —  Application
| Number | Deliverable | Specification |
|-|-|-|
| 0 | Application | We will consider its application for Vechain's ecosystem (e.g., improving PoA 2.0's finality) |

## Budget

The money is used for living supplies as well as infrastructures that will be needed for building the prototype and evaluation on Cloud.

For each Milestone, the budget is $ 10,000, and $ 30,000 in total.

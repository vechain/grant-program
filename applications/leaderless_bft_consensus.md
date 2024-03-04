# VeChain grant research proposal template

## Leaderless Byzantine Fault Tolerant Consensus

## Applicants

Fangyu Gai (corresponding applicant). He is currently a third-year Ph.D. student at School of Engineering, University of British Columbia, supervised by [Dr. Chen Feng](https://people.ok.ubc.ca/cfeng01/index.html), who is the co-cluster lead of [Blockchain@UBC](https://blockchain.ubc.ca/). His research interests lie in distributed systems, especially blockchain systems. Most recently, He has been focusing on building efficient and high-performance permissioned blockchain databases at [Alibaba DAMO Academy](https://damo.alibaba.com/) as a research intern. More information including his CV can be found at his [website](https://fangyugai.me/).

Jianyu Niu. He is currently a fourth-year Ph.D student at School of Engineering, University of British Columbia, also supervised by Dr. Chen Feng. His research interests focus on incentive and consensus protocol designs on blockchains. His CV can be found [here](https://fangyugai.me/files/JiangyuNiu_CV.pdf).

Chen Feng. He is an assistant professor and Tier-2 principal’s research chair in Blockchain in the University of British Columbia and he is also the co-cluster lead of [Blockchain@UBC](https://blockchain.ubc.ca/). His research interests include information and coding theory, wireless communications and networking, cloud computing and big data, and very recently blockchain technology. In particular, he is interested in adapting new ideas and tools from information theory, coding theory, stochastic processes, and optimization to design better communication networks with a particular emphasis on quantum communications and blockchain technology. The primary goal of his research is to bridge the gap between theoretical advances and system implementations. For more information about him (including his CV), please visit his [website](https://people.ok.ubc.ca/cfeng01/index.html).

## Payment Address

USDT: 0x0157982d81b408E180545277Fa2104490cB46ae9

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
| Estimated Duration | 60 d | 60 d | 60 d | 180 d |
| Full-time equivalent (FTE) | 0.5 | 0.5 | 0.5 | 1.5 |
| Cost (up to $ 30,000) | $ 5,000 | $ 5,100 | $ 5,100 | $15,200 |

#### Milestone 1 — Scientific paper

| Number | Deliverable | Specification |
|-|-|-|
| 0 | Techinical Report | We will improve the technical report that we have been writing and make sure it is well-written and technically correct; the output should be a techinical report publicly available on [arXiv](https://arxiv.org/) and potentially submitted to some academic conference or journal |

#### Milestone 2  —  Prototype
| Number | Deliverable | Specification |
|-|-|-|
| 0 | Open-sourced Demo | We will build a prototype of our protocol using Golang for proof-of-concept; the output should be a open-sourced repo on [github.com](https://github.com/) that is implemented following the specification of the technical report from Milestone 1 and have cloud-deployment abilities |

#### Milestone 3  —  Application
| Number | Deliverable | Specification |
|-|-|-|
| 0 | Integrated Blockchain Platform | We will consider its application for Vechain's ecosystem (e.g., improving PoA 2.0's finality); the output should be production-level code integrated into an existing blockchain platform |

## Budget

The budgest mainly consists of human resources and cloud facilities.

According to UBC's latest teaching assistant [pay rate](https://cupe2278.ca/how-we-help/pay-rates/), a Ph.D. student is paid at the level of GTA I, which is 34.44 CAD (around 29 USD) per hour. For each milestone, we have 60 days, which is 8.5 weeks, counting to 8.5 (weeks) * 40 (total work hours per week) * 0.5 (FTE) = 170 h. Therefore, the budget for human resources is 170 * 29 = 4,930, which is up to 5k USD.

As for the cloud deployment facilities that will be used in Milestone 2 and 3, the budget is calculated based on the hourly price of AWS's EC2 [instance a1.xlarge](https://aws.amazon.com/ec2/pricing/on-demand/):
0.1 (hourly price) * 10 (instance number) * 100 (expected hours) = 100 USD.

In summary, the budget for Milestone 1, 2, 3 is 5,000 USD, 5,100 USD, and 5,100 USD, respectively.

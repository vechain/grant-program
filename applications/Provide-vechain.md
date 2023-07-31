# VeChain General Grant Application Template

## Project Overview 

- Project: PRVD Stack Interopability to VeChain
- Team Name: Provide Technologies Inc
- Payment Address: USDC (ERC 20) payment address. 0xE62A9086ac0536057FFA23Ea57a3038Fe601186D

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

The Provide platform enables enterprise apps like SAP and Service and other web2 applications in Node.js, .NET, Python to integrate to blockchains. 

A key feature of the Provide platform is our implementation of the Baseline Protocol, known as the Provide Axiom API. 

[Axiom](https://docs.provide.services/axiom) - together with our low code designer [Shuttle](https://shuttle.provide.services) enables developers and business analysts to easy create workflows based on zero knowledge proofs. 
Axiom and Shuttle together make zero knowledge <i>composable</i>.

Other components of the Provide platform include these APIs as well
[Ident](https://docs.provide.services/ident) - microservice providing decentralized identity, authentication and authorization services
[Vault](https://docs.provide.services/vault) - Digital wallet and cryptographic secrets management
[Nchain](https:/docs.provide.serivces/nchain) - Smart contract middleware for multiple public and private networks
[Privacy](https://docs.provide.services/privacy) - General purpose ZK api, used as a subcomponent to Axiom. Can be used on a standalone basis for zk proof creation and verificatoin.

We are interested to participate in the VeChain ecosystem because we feel VeChain's core enterprise user group would take interest in our connectors to SAP and ServiceNow. 
The Provide wallet-as-a-service offering with the Vault and Nchain APIs enable rapid blockchain integration that native embeds inside of enterprise apps - and we consider this a highly attractive for F500s and other SMB business users.

The Axiom API also helps address many data privacy and precision problems that can occur either on or off chain. 
The Axiom zk-proofs of certain business processes could also be considered oraclized data inputs for real world assets like ERP invoices and AR/AP balances. 
Axiom also broadens ZK from a blockchain privacy/scaling technique into a general purpose integration pattern - forging a new frontier in cross-company workflows in domains like suppy chain, ESG, finance, and more.

These offerings altogether can help grow VeChain's ecosystem of enterprise users. Shuttle as a ZK low/no-code tool may also later prove a valuable complement to Vorj.app for enterprise developers.

Introducing the Provide platform to VeChain also leads the to possibility to later integrate our zk-rollup and zkEVM to VeChain, thereby introducing the possibility of launching a layer 2 upon VeChain.

We also highly value VeChain's commitment to engage with enterprises goals and duties in the sustainability domain. We share a similar vision on blockchain enables corporates to synchronize ESG data and help drive climate investments globally to where most urgently needed.

Our overall goal with this grant is to lay the technical foundations to fully support VeChain throughout our entire API stack. 
A secondary goal we have to is to share our VeChain integration with a business audience not ordinarily exposed to blockchain / digital assets - such as an event focused on SAP / ServiceNow / Corporate ESG users.

### Project Details

We'd like to add VeChain support throughout the Provide platform that other EVM networks benefit from (ex: Ethereum, Polygon, Celo) - prioritizing adaptation of the Connex / Thorify APIs to the Provide Nchain component. 

Because VeChain's APIs have some differences to other EVM-compatible networks' JSON-RPC, there will be some additional development to achieve full interopability with the Provide Nchain component.
However - as both Provide Nchain and the VeChain APIs are written Golang, the adaptation should remain straightforward.

Once this is completed - a broad range of other very excitying apps immediately become interopable with VeChain. 

This includes Node.js and SAP ABAP projects we've prototyped that can send stablecoins/ERC-20s/CBDCs and mint NFTs.



This also enables us to more easily deploy ZK-based Solidity contracts that are generated from Provide Shuttle, Axiom, and Privacy to VeChain

We expect the teams to already have a solid idea about the project's expected final state.
Therefore, we ask the teams to submit (where relevant):
- Mockups/designs of any UI components
- API specifications of the core functionality
- An overview of the technology stack to be used
- Documentation of core components, protocols, architecture, etc. to be deployed
- PoC/MVP or other relevant prior work or research on the topic

### Ecosystem Fit
There are several other startups building middleware between blockchains and enterprise systems. We stand apart from others because the core of our technology solution is open source. 
We're also highly differentiated with our approach to zero knowledge.

## Team 

### Team members

- Ryan Fleischmann
- Kyle Thomas

### Team Website

- https://provide.services

### Team's experience

Please describe the team's relevant experience. If the project involves development work, then we'd appreciated it if you can single out a few interesting codes commits made by team members on their past projects. 

### Team Code Repos

- https://github.com/<your_repo_1>
- https://github.com/<your_repo_2>

### Team LinkedIn Profiles

[Ryan](https://www.linkedin.com/in/ryan-fleischmann-3aa59712/)
[Kyle](https://www.linkedin.com/in/kylebthomas/)


## Development Roadmap 

This section should break out the development roadmap into a number of milestones. Since the milestones will appear in the grant contract, it helps to describe the functionality we should expect, plus how we can check that such functionality exists in the product. Whenever milestones are delivered, we refer to the contract to ensure that everything has been delivered as expected.

Below we provide an <b>example roadmap</b>. For each milestone:

- Please indicate the milestone duration, workload in terms of full-time equivalent (FTE) and cost. 
- Please be sure to include a specification of the software. The level of details must be high enough so that we are able to verify that the software meets the specification.
- Please note that we require documentation (e.g. tutorials, API specifications, architecture details) in each milestone. This ensures that the code can be widely used by the community.
- Please provide a test suite, comprising unit and integration tests, along with a guide on how to run these.
- Please commit to providing dockerfiles for the delivery of your project.


### Example Roadmap for a dApp Application

#### Overview

|  | Milestone 1 | Milestone 2 | Total |
| - | - |- | - |
| Estimated Duration | 30 d | 30 d | 60 d |
| Full-time equivalent (FTE) | 2 | 1 | 3 |
| Cost (up to $ 30,000) | $ 5,000 | $ 10,000 | $ 15,000|

#### Milestone 1 — Smart Contract & Backend

| Number | Deliverable | Specification |
|-|-|-|
Integrate Provide Vault to VeChain Connex/Thorify
Adapt the VeChain Connex/Thorify APIs to Provide Nchain, test existing apps
Test Provide Axiom zk-proof propagation to VeChain
| 0a.| License | Apache 2.0 / MIT / Unlicense |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial that can interact with the deployed smart contracts and backend service. |
| 0c. | Testing Guide | The code will have proper unit-test coverage (e.g. 90%) to ensure functionality and robustness. In the guide, we will describe how to run these tests |
| 1 | Smart Contracts | We will develop smart contracts that will...  (Please list the functionality that will be coded for the contracts) . We will open source the smart contract and upload the ABI to [B32](https://github.com/vechain/b32). |
| 2 | Backend | "We will create a backend service that will... (Please list the functionality that will be coded for the backend)" |

#### Milestone 2  —  Frontend
| Number | Deliverable | Specification |
|-|-|-|
| 1 | User Guide | We will provide a user guide or a demo video to show what features have been done.  |
...

#### Community engagement

As part of the Program, we require that you produce and publish at least one article/tutorial (e.g., on Medium). It should explain your work done as part of the grant. 

Our docs: https://docs.provide.services
Twitter https://twitter.com/provideplatform
Discord https://discord.gg/VG7JPFS5tk
Telegram https://t.me/provideofficial
Github https://github.com/provideplatform

## Future Plans

Provide aims to be protocol agnostic, but we're generally interested to support ecosystems with a high commitment to zero knowledge, enterprise, and sustainability.
We want to grow our network of customers using our commercial support of these APIs so that we can launch the Provide Network - our zkEVM/zk-rollup

## Additional Information 

Any additional information that you think is relevant to this application that hasn't already been included.

Possible additional information to include:
- Ryan Fleischmann of Provide is a recipient of the VeChain developer microgrant
- We have been supported by a network of investors. We also have a strategic partnership with KlimaDAO/Carbonmark

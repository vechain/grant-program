# Provide platform integration to VeChain

## Project Overview 

- Project: Provide platform integration to VeChain
- Team Name: Provide Technologies Inc
- Payment Address: USDC (ERC 20) payment address. 0xE62A9086ac0536057FFA23Ea57a3038Fe601186D

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

The Provide platform enables enterprise apps like SAP and Service and other web2 applications in Node.js, .NET, Python to integrate to blockchains such as VeChain.

A key feature of the Provide platform is our implementation of the Baseline Protocol, known as the Provide Axiom API. 

[Axiom](https://docs.provide.services/axiom) - together with our low code designer [Shuttle](https://shuttle.provide.services) enables developers and business analysts to easy create workflows based on zero knowledge proofs. 
Axiom and Shuttle together make zero knowledge <i>composable</i> - neutralizing the knowledge and skills barriers developers struggle with in adopting ZK.

Pictured below - a sample Axiom API call generating the zk-proof on-demand in Postman, and the corresponding workstep configuration

![ZK proof created based on Shuttle zk-workflow](https://github.com/fleischr/baseline/blob/bpi-interop/create-bri1-msg-example/examples/bpi-interop/scripts/bri-1/img/postman-sent-protocol-msg.PNG)

![Provide Shuttle ZK-workflow designer](https://github.com/fleischr/baseline/blob/bpi-interop/create-bri1-msg-example/examples/bpi-interop/scripts/bri-1/img/shuttle-msg-review1.PNG)

![ZK-workstep in Provide Shuttle. Simply define data schema input you need zk-proofed, what kind of circuit is need, who needs to participate in the zk-workflow, configure if Layer1 finality is required](https://github.com/fleischr/baseline/blob/bpi-interop/create-bri1-msg-example/examples/bpi-interop/scripts/bri-1/img/wf-workstepsave.PNG)


Other components of the Provide platform include these APIs as well

[Ident](https://docs.provide.services/ident) - microservice providing decentralized identity, authentication and authorization services

[Vault](https://docs.provide.services/vault) - Digital wallet and cryptographic secrets management

[Nchain](https:/docs.provide.serivces/nchain) - Smart contract middleware for multiple public and private networks

[Privacy](https://docs.provide.services/privacy) - General purpose ZK api, used as a subcomponent to Axiom. Can be used on a standalone basis for zk proof creation and verificatoin.

We are interested to participate in the VeChain ecosystem because we feel VeChain's core enterprise user group would take interest in our connectors to SAP and ServiceNow, zk capabilities, and wallet-as-a-service offering. 
The Provide wallet-as-a-service offering with the Vault and Nchain APIs enable rapid blockchain integration that native embeds inside of enterprise apps - and we consider this a highly attractive for F500s and other SMB business users.

Provide's zero knowledge capabiliities are led by Axiom, our implementation of the [Baseline Protocol standard](https://baseline-protocol.org). The Axiom API also helps address many data privacy and precision problems that can occur either on or off chain. 
The Axiom zk-proofs of certain business processes could also be considered oraclized data inputs for real world assets like ERP invoices and AR/AP balances. 
Axiom also broadens ZK from a blockchain privacy/scaling technique into a general purpose integration pattern - forging a new frontier in cross-company workflows in domains like suppy chain, ESG, finance, CRM, and more.

These offerings altogether can help grow VeChain's ecosystem of enterprise users. Shuttle as a ZK low/no-code tool may also later prove a valuable complement to Vorj.app for enterprise developers.

Introducing the Provide platform to VeChain also leads the to possibility to later integrate our zk-rollup and zkEVM to VeChain, thereby introducing the possibility for Provide to assist in launching a layer 2 upon VeChain in the future.

We also highly value VeChain's commitment to engage with enterprises goals and duties in the sustainability domain. We share a similar vision on blockchain enables corporates to synchronize ESG data and help drive climate investments globally to where most urgently needed.

Our overall goal with this grant is to lay the technical foundations to fully support VeChain throughout our entire API stack. 
A secondary goal we have to is to share our VeChain integration with a business audience not ordinarily exposed to blockchain / digital assets - such as an event focused on SAP / ServiceNow / Corporate ESG users.

### Project Details

We'd like to add VeChain support throughout the Provide platform that other EVM networks benefit from (ex: Ethereum, Polygon, Celo) - prioritizing adaptation of the Connex / Thorify APIs to the Provide Nchain component. 

Because VeChain's APIs have some differences to other EVM-compatible networks' JSON-RPC, there will be some additional development to achieve full interopability with the Provide Nchain component.
However - as both Provide Nchain and the VeChain APIs are written Golang, the adaptation should remain straightforward.

Once this is completed - a broad range of other very exciting apps immediately become interopable with VeChain. 

This includes Node.js and SAP ABAP projects we've prototyped that can send stablecoins/ERC-20s/CBDCs and mint NFTs. Developers using the Provide APIs simply need to reference the VeChain.

Our overall deliverable is for our existing open source resources to reflect support (Provide platform APIs: Ident, Vault, Axiom, Nchain, Privacy) for VeChain with several supporting repos and documentation samples. At least one example should prototype the use zero knowledge from the Provide platform API stack.

The deliverables described shall later enable us to more easily deploy ZK-based Solidity contracts that are generated from Provide Shuttle, Axiom, and Privacy to VeChain

### Ecosystem Fit

There are several other startups building middleware between blockchains and enterprise systems. We stand apart from others because the core of our technology solution is open source. 
We're also highly differentiated with our approach to zero knowledge.

## Team 

### Team members

- Ryan Fleischmann (Developer Relations, JS/SAP architect)
- Kyle Thomas (CEO/CTO)
- Benjamin Bukari (COO/Legal)

### Team Website

- https://provide.services

### Team's experience

Please describe the team's relevant experience. If the project involves development work, then we'd appreciated it if you can single out a few interesting codes commits made by team members on their past projects. 

### Team Code Repos

See our github organization

https://github.com/provideplatform

We offer nearly 40 repositories that collectively represent the entirity of the Provide platform. However the 5 core microservices

### Team LinkedIn Profiles

[Ryan Fleischmann](https://www.linkedin.com/in/ryan-fleischmann-3aa59712/)

[Kyle Thomas](https://www.linkedin.com/in/kylebthomas/)


## Development Roadmap 

#### Overview

Cost $30,000
FTE equivalent 2

We anticipate to complete all 4 milestones in next 60 days
To cover some operations cost of our stack and SAP dev environment - we're requesting  $10k of the grant to be awarded upfront, with $5k awarded upon each milestones completion.

#### Milestone 1 — Integrate Provide Vault directly to VeChain Connex/Thorify API

Provide Vault can already produce hashed, digitally signed data from secp256k1 keys that can be directly broadcast to the VeChain APIs.

Our goal will be to create test applications that leverages the VeChain REST interface in this manner leveraging our current sample repos that demonstrate the usage of the Provide APIs

Current provide-js sample repos:
- [Send an ERC-20 with provide-js](https://github.com/fleischr/transfer-erc20-providejs)
- [Mint an NFT with provide-js](https://github.com/fleischr/mint-nft-provide-js)

Upon successful integration with the provide-js SDK samples, we'd like to attempt to the the same with corresponding sample repos for [provide-abap](https://github.com/provideplatform/provide-abap) - our SDK for SAP S/4 HANA
- [ABAP ERC-20](https://github.com/fleischr/abap-erc-20)
- [ABAP NFT](https://github.com/fleischr/abap-nft)

This establishes a MVP in terms Provide - VeChain integration going forward.

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Fork provide.js apps with VeChain REST | Provide Nchain may not be immediately usable - but the signing/broadcasting should still work |
| 2 | Fork provide-abap apps with VeChain REST | Provide Nchain may not be immediately usable - but the signing/broadcasting should still work |
...

#### Milestone 2  —  Adapt the VeChain Connex/Thorify APIs to Provide Nchain, test existing apps

To promote greater interoperability and general Provide platform developer user experience, we want to fully abstract the VeChain APIs into Provide Nchain. This will enable developers using the Provide platform for other Ethereum ecosystem blockchains to transition to integration on VeChain more easily. This makes our long term maintenance and support of VeChain more straightforward.

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Provide NChain - VeChain Golang adapter | We will use golang to add some middleware code to Provide Nchain that enables developers to send transactions to VeChain nodes in the same way that Provide Nchain sends transactions to JSON-RPC. Golang is used both in Provide Nchain and VeChain SDK, we anticipate the technical build to be rather straightforward |
| 2 | Document advantages of this approach | How does this benefit Provide-VeChain users in terms of end to end technical support? Examples may include: how this gives enterprises greater access controls to wallets, upgraded Axiom and DID/SSI capabilities and built in support products like our fiat-crypto bridge Provide Payments |
...

#### Milestone 3  —  ZK input for/output for real world transaction
For milestone 3, we'd like to begin to demonstrate our POV on use of ZK in real world asset tokenization. An Axiom zero knowledge proof generated from a mock business process (e.g. paying an invoice, goods receiving a product in a manufacturing facility) will be used as an input data for a custom-built NFT that retains those proofs for verification onchain.

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Create user guide | Explain how to create the zk-workflow in Provide Shutte and Axiom and how the proofs flow into VeChain based assets |
| 2 | App build | Build open source reference app that uses the Axiom zk-workflow in tokenization |
| 3 | Non-technical user summary / blog | Explain the role of ZK in approachable business terms in how it helps notarize real world data inputs with data privacy and precision - and how this fits the ethos of the VeChain ecoysystem |
...

At least 1 new github repository with the configuration instructions, Postman collection, and sample source code will be provided.

#### Milestone 4 - Share the Provide platform capabilities on VeChain to business / IT audience 
| Number | Deliverable | Specification |
|-|-|-|
| 1 | Create one-pager | Summarize the Provide Platform capabilities available on VeChain and their value to the ecosystem |
| 2 | Public event | We'd be glad to share a live demo at a professional services oriented event for CEOs/CIOs/CFOs and other business IT executives |
| 3 | Provide Architecture Q&A | Share high level details for technical admins on how to deploy the Provide system architecture to run the Provide APIs and apps. |
...

#### Community engagement

Our docs https://docs.provide.services

Twitter https://twitter.com/provideplatform

Discord https://discord.gg/VG7JPFS5tk

Telegram https://t.me/provideofficial

Github https://github.com/provideplatform

Youtube https://www.youtube.com/@providetechnologies7488

## Future Plans

Provide aims to be protocol agnostic, but we're generally interested to support ecosystems with a high commitment to zero knowledge, enterprise, and sustainability.
We want to grow our network of customers using our commercial support of these APIs so that we can launch the Provide Network - our zkEVM/zk-rollup. Assuming we can add layer 1 finality to VeChain to this zk-rollup, we can foresee the VeChain enterprise user community to be a frequent user of this capability.

## Additional Information 

Possible additional information to include:
- [Ryan Fleischmann](https://twitter.com/RyFleisch) of Provide is a recipient of the VeChain developer microgrant for the Carbon Emissions NFT
- We have been supported by a network of investors. We also have an active strategic partnership with KlimaDAO/Carbonmark

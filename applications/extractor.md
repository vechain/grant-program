# Extractor - VeChain General Grant Application

## Project Overview 

- Project: __Extractor__
- Team Name: Hacken OU
- Payment Address: 0xe159c80850fba5d34a34a9f18bed089d3c1be929 (USDC ERC-20).


### Overview

__Extractor__ is a Post Deployment security solution that provides multi-level asset protection (smart contract, transaction monitoring, and security tool) against on-chain attacks and vulnerabilities exploits

__Extractor__'s mission is to make Web3 a safer place. By integrating our product into VeChain Ecosystem all projects would be able to use more advanced security solutions and protect their assets.

### Project Details

The product is live in production: https://extractor.hacken.io

High Level Architectural Diagram:

<img src="https://github.com/haas-labs/extractor/raw/main/doc/Ext-Architecture.png" width="800">

<br>

Examples of screens (access to Figma with Full design deck can be provided):

<img src="https://github.com/haas-labs/extractor/raw/main/doc/Ext-Screen-1.png" width="800">

<br>
<img src="https://github.com/haas-labs/extractor/raw/main/doc/Ext-Screen-2.png" width="800">

<br>
<img src="https://github.com/haas-labs/extractor/raw/main/doc/Ext-Screen-3.png" width="800">

<br>
<img src="https://github.com/haas-labs/extractor/raw/main/doc/Ext-Screen-4.png" width="800">

<br>

__Brief Product Slidedeck__:

[Extractor-VeChain.pdf](https://github.com/haas-labs/extractor/blob/main/doc/Extractor-VeChain.pdf)


### Ecosystem Fit

Having extensive security experience in the EVM ecosystem both with Smart contracts Audits and automated on-chain detection and protection we bring this capability to the VeChain world by integrating with Extractor. 

Our clients do not need to put in any technical effort as the Extractor team is helping with the product activation and monitoring with no code solution. 

We provide complete protection coverage with the possibility of implementing automatic Smart Contract Actions.


## Team 

### Team members

The team will comprise of 3 core engineers:

- Team Lead:  Andriy K, (https://github.com/andriyk-hacken)

- 1 Blockchain Ingest/Integration Data Engineer: Andriy U (https://github.com/)

- 1 BackEnd Developer: Gleb K (https://github.com/gkozyryatskyy)

- 1 Front-End developer: Vova G (https://github.com/vgutorov-hacken)

Support roles:

- Product Owner (Denys I)

### Team Website

- https://extractor.hacken.io

### Team's experience

The team has extensive experience building SaaS web2 and web3 infrastructure products. During the last 1.5 years, the team was involved in building BigData data ingestion and analytics for web3 security.

Members of the team have been at the roots of the Layer-1 Protocol Audit service business.


### Team Code Repos

The project is currently in private repositories. We will invite to repositories at your request.

### Team LinkedIn Profiles

- Andriy K (https://www.linkedin.com/in/andriy-kashcheyev-a019382/)
- Andriy U (https://www.linkedin.com/in/andreyusov/)
- Gleb K (https://www.linkedin.com/in/gleb-kozyryatskyy-51074395/)
- Vova G (https://www.linkedin.com/in/vlgutv/)


## Development Roadmap 

#### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3 | Total |
| - | - |- | - | - |
| Estimated Duration | 30 d | 30 d | 20 d |80 d |
| Full-time equivalent (FTE) | 1 | 3 | 2 | 6 |
| Cost  | $ 7,000 | $ 15,000 | $ 8,000| $ 30,000|

#### Milestone 1 - VeChain Ingestion Engine

| Number | Deliverable | Specification |
|-|-|-|
| 1.| Node RPC Interface | Implementation of VeChain RPC spec interface to retrieve and parse data from node for the following entities: blocks, transactions, transfers, event logs.  |
| 2. | Ingest Streaming | Implementation of real-time streaming (Kafka Connect pipelines). |
| 3. | Token transfers | Implementation of Asset transfers ingestion (ERC-20, NFT). |

#### Milestone 2 - Extractor Interceptor Integration

| Number | Deliverable | Specification |
|-|-|-|
| 1.| VeChain data mapping  | Implementation of VeChain data entities and fields mapping to internal Script Engine to evaluate fields from scripts.  |
| 2. | Token Transfer Interceptor | Implementation of Token Transfer Trigger with supported event types (e.g. Approve, Transfer, ..) |
| 3. | Blacklist and Whitelist Interceptor | Implementation of Blacklist and Whitelist Addresses (EOA and Contracts) Trigger function |
| 4. | Event Log Interceptor | Implementation of arbitrary Receipt Log Trigger with a predefined ABI list templates |
| 5. | Failed Transaction Interceptor | Implementation of failed transactions Trigger. |

#### Milestone 3 - Advanced Interceptors

| Number | Deliverable | Specification |
|-|-|-|
| 1.| ABI Database | Implementation of ABI Contract and Event logs signatures for Transaction and Receipts decoding. |
| 2. | Function Calls Decoder | Implementation of Contract function call (parameters and types) decoder |
| 3. | Function Call Interceptor | Implementation of failed transactions Trigger |


#### Community engagement

Updates and articles are regularly published on all company social feeds:

- https://www.linkedin.com/company/hacken/
- https://t.me/hackenai
- https://twitter.com/hackenclub
- https://hacken.io/hacken-news


Example of the article: https://hacken.io/hacken-news/hacken-extractor-update/

We are committed to publish several artciles and udpdate on VeChain integration and how Product works on VeChain ecosystem.


## Future Plans

Our roadmap includes a number of new integrated blockchains and how product capabilities can be extended by independent teams or members (like Auditors or White hackers).

We are planning to provide SDK and capability to implement complex long range attack detection and correlation with off-chain events in Attack Detector module with Automatic Actions (contract transactions).

Roadmap includes monitoring and trigger of tokenomics changes (e.g. Circulation Supply) and other higher business metrics

On-chain data analysis to build more robust detection models with low false positives is a primary objective for automated protection.


## Additional Information 

Our current product is live in production for EVM chains (https://extractor.hacken.io). The development has been self-funded so far.

We have already a number of paying clients and actively promoting to new clients.

Our roadmap includes intergration with non-EVM chains and we are carefully evaluating which another blockchain to integrate with and apply for a grant.

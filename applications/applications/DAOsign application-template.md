# VeChain General Grant Application Template

## Project Overview 

- Project: DAOsign
- Team Name: DAOsign 
- Payment Address: 0x793F7a7542c14088dbF58A19d2687FB9E7A79482

### Overview

DAOsign is a decentralized platform for agreements and automated workflows, with publicly verifiable, cryptographic proofs-of-signature, designed for DAOs and WEB3 companies.

Verifiable Signature is at the core of DAOsign and is based on 3 key proofs: proof-of-identify, proof-of-authority, and proof-of-agreement. Utilizing these proofs, DAOsign provides a platform to design and configure complex workflows that combine smart-contract-based automation with authorized approvals.

DAOsign addresses the need for a secure and transparent way to sign, manage and automate agreements of all kinds with a configurable level of anonymity disclosure.

### Project Details

**Core DAOsign components**![image](https://github.com/TetianaRiabova/grant-program/assets/122782612/69a01978-5c7f-4997-85e4-00ad86e216d5)

**Technical design**

Proofs are implemented in the EIP-712 standard and adjusted to ink! ecosystem. Proofs digned using user’s EVM private key. We are supporting this standard in Ink! smart contract to be able to verify the signature in ink! smart contract. Also, we are implementing an adjusted EIP-2771 standard to allow Agreement Signers gas-free delegation to publish proof on-chain. EIP-712 standard will be used for proofs, adaptation means that user data is converted to a binary bit; we use its hash (serialization vs deserialization) And EIP-2771 standard - to securely send the proof and receive it. So that EVM standards will be adapted to ink! ecosystem requirements. Example (interfaces) of the smart contracts can be found here https://github.com/DAOsign/daosign-smart-contracts (Solidity version).

Detailed storyboard can be found here: https://consideritdone.storiesonboard.com/m/PUCLDvQC4kKwoRJ8kbm3MA .

**Architectural diagram**![image](https://github.com/TetianaRiabova/grant-program/assets/122782612/789d821d-86c8-4a55-b174-aad4b86214bc)

Agreement Proof entity represents 3 proofs:

- Proof of signature

- Proof of authority

- Proof of agreement

The detailed Proof Technical Design is [here](https://github.com/w3f/Grants-Program/files/12183424/Proofs.Technical.Design.-.DAOSign.pdf)



Pitch Deck: https://docsend.com/view/sbexkxn5su3ahdg8

One-pager: https://drive.google.com/file/d/1lDWNBoz18y11kARGxZpQrN_ca2muDmT7/view?usp=sharing

### Ecosystem Fit

We believe that DAOsign can benefit the Vechain ecosystem by enhancing governance, fostering collaboration, expanding use cases, ensuring trust and security, and promoting cross-chain compatibility.

We have 2 categories of competitors: legacy electronic signature tools such as DocuSign and web3 signature tools such as ethsign.xyz. We have made some research and you can find the detailed competitive landscape in the one-pager above. 

## Team 

### Team members

Eugene Fine - CEO & Founder

Ramil Amerzyanov - CTO

Misha Kushka - Technical Lead

Oleksandra Burmenska - Business Development Director

### Team Website

https://daosign.org/

### Team's experience

**Eugene Fine**: CEO, Founder Background: Over 20 years of building, scaling, and managing technology organizations. Past experience:

- CTO for https://www.explorersurgical.com
- tech leadership contribution to https://bird.coach
- tech advisor and facilitator for polywrap.io to name a few. Also, Eugene is a founder at consideritdone.tech and daosign.org


**Ramil Amerzyanov**: Solution Architect, CTO Background: 15+ years in building complex enterprize solutions (all SDLC aspects), including 7+ years in Blockchain industry. Past projects include:

- contribution to Ethereum standards development
- tech leadership for https://docsend.com/view/fjrvjtyzgm7wgrkj projects

**Oleksandra Burmenska**: Director of Business Development and Partnerships Background: Engineering, MBA, and Psychology diplomas. Over a decade of experience in IT: development and managerial positions, last five years focused on the Blockchain industry. Experience with enterprises and startup companies, scaling teams, and building blockchain products. Previous blockchain projects include:

- successfully managed ICOs during 2017-2019 (example: Õpet – Medium )
- contribution to Polywrap, NEAR, Axelar, GnosisSafe, Avalanche ecosystems
- contribution to nodle.com ecosystem: managing the block explorer development (before it moved to Subscan), leading the Landslide - Avalanche subnet development,etc.

**Misha Kushka**: Tech Lead and Blockchain Developer Background: 6+ years of professional experience as a developer, 4+ years of professional experience in the Blockchain field, 4+ years experience as a lead

Our portfolio: https://docsend.com/view/fjrvjtyzgm7wgrkj
 

### Team Code Repos

https://github.com/ConsiderItDone,

https://github.com/ramilexe,

https://github.com/kushkamisha,

https://github.com/burmenska

### Team LinkedIn Profiles

https://www.linkedin.com/in/eugenefine/

https://www.linkedin.com/in/ramil-amerzyanov/

https://www.linkedin.com/in/mkushka/

https://www.linkedin.com/in/oleksandra-burmenska/

## Development Roadmap 

MVP on Testnet - Q2 2023

Blockchain Integration - Q2 2023

Snapshot + GPT3 Integration - Q3 2023 

Agreement Invoicing - Q3 2023 

Plugins Marketplace and Tokenization - Q4 2023


#### Community engagement

Twitter: https://twitter.com/dao_sign

LinkedIn: https://www.linkedin.com/company/daosign/

Discord: https://discord.gg/AwnhGFbT8Z

Telegram: https://t.me/DAOsign

Please, take a look at our community statistics [here](https://docs.google.com/document/d/16rOe-6r-mftePwb_88IU6iOkRCEA1cxu1FNcE5Ep4uA/edit?usp=sharing)

# VeChain General Grant Application Template

## Project Overview 

- Project: DAOsign
- Team Name: DAOsign 
- Payment Address: 0x793F7a7542c14088dbF58A19d2687FB9E7A79482

### Overview

DAOsign is a smart signature and workflow automation platform, with publicly verifiable, cryptographic proofs-of-signature, designed for DAOs and WEB3 companies.

Verifiable Signature is at the core of DAOsign and is based on 3 key proofs: proof-of-identify, proof-of-authority, and proof-of-agreement. Utilizing these proofs, DAOsign provides a platform to design and configure complex workflows that combine smart-contract-based automation with authorized approvals.

One of the most important features of blockchain is privacy and the ability to remain anonymous, especially when it comes to signing important documents. One of the reasons that motivated us to create DAOsign is our previous work as a consulting agency. We often encountered a situation where signing legal agreements with clients was challenging because they did not want to reveal their identities. Neither DocuSign nor other signature platforms could solve this problem. Subsequently, we decided to create a product that addresses the need for a secure and transparent way to sign, manage, and automate agreements of all kinds with a configurable level of anonymity disclosure. 

DAOsign is blockchain agnostic, so users can choose where to store the proofs. DAOsign already allows users to store proofs of signature in the IPFS, Ethereum launch is planned in the nearest time. Also, recently, we received grants from SUI and Polkadot, so DAOsign users will be able to use these blockchains for proofs storing purposes soon as well.

Furthermore, DAOsign provides a robust Governance and Policy Builder platform to offer governance, workflow automation, and controls for organizational policies and procedures.

We also recently discovered and implemented a use case for commodity trading (grain trading), which shows that DAOsign goes beyond web3 and can also be used in web2.

These features and use cases (our team continues to work on to increase their number) are essential for any ecosystem that strives for improved privacy and security.

We suggest watching a demo for a better understanding of how DAOsign works: https://www.youtube.com/watch?v=FdctkL6eShw

And we invite you to try our platform on the Testnet: https://testnet.daosign.org/

### Project Details

**Core DAOsign components**![image](https://github.com/TetianaRiabova/grant-program/assets/122782612/69a01978-5c7f-4997-85e4-00ad86e216d5)

**DAOsign Stack** ![image](https://github.com/TetianaRiabova/grant-program/assets/122782612/4a0ad112-78c9-43cd-b88e-e9f374b60912)

**Architectural diagram**![image](https://github.com/TetianaRiabova/grant-program/assets/122782612/789d821d-86c8-4a55-b174-aad4b86214bc)

Agreement Proof entity represents 3 proofs:

- Proof of signature

- Proof of authority

- Proof of agreement

The detailed Proof Technical Design is [here](https://github.com/w3f/Grants-Program/files/12183424/Proofs.Technical.Design.-.DAOSign.pdf)


Pitch Deck: https://docsend.com/view/sbexkxn5su3ahdg8


### Ecosystem Fit

We believe that DAOsign can seamlessly integrate into the Vechain ecosystem by providing a platform to manage decision-making processes in a decentralized manner. Our target audience extends beyond DAOs to include all companies that need to handle agreement/policy management, including the use case for managing Grants, which you can find in our pitch deck. The goal of this use ase is to simplify all stages of the funding process. We didn't find any similar projects in Vechain Ecosystem.

We have 2 categories of competitors: legacy electronic signature tools such as DocuSign and web3 signature tools such as ethsign.xyz. We have made a detailed research and you can find the competitive landscape in the pitch deck above.

## Team 

### Team members

Eugene Fine - CEO & Founder

Ramil Amerzyanov - CTO

Misha Kushka - Technical Lead

Oleksandra Burmenska - Head of Partnerhips

### Team Website

https://daosign.org/

### Team's experience

**Eugene Fine (CEO & Founder)** - Over 20 years of building, scaling, and managing technology organizations. Recent experience includes a CTO role at Explorer Surgical Corp., which was recently acquired by GHX, and VP of Engineering at GHX. Eugene is a founder at consideritdone.tech, a Blockchain/WEB3 development studio.
GitHub: https://github.com/ConsiderItDone
LinkedIn link: https://www.linkedin.com/in/eugenefine/

**Ramil Amerzyanov (CTO)** - 15+ years building complex technical architecture and software solutions., focusing on Blockchain/WEB3 technologies over the past 7 years. Recent projects include the Fractional CTO role at Landslide Network and CTO role at consideritdone.tech.
GitHub: https://github.com/ramilexe
LinkedIn link: https://www.linkedin.com/in/ramil-amerzyanov/


**Misha Kushka (Technical Lead)** - 6+ years developing Blockchain/WEB3 technical architecture and software solutions. Recent projects include Lead Technical Architect roles at Akiva Capita! Holdings and Avalanche
GitHub: https://github.com/kushkamisha


**Oleksandra Burmenska (Head of Partnerships)** - Over 10 years of experience in Business Development and Management roles in Technology organizations, focusing on Blockchain/WEB3 technologies over the past 5 years. Recent projects include contributions to NEAR, Axelar, GnosisSafe, and Avalanche ecosystems.
GitHub: github.com/burmenska
LinkedIn link: https://www.linkedin.com/in/oleksandra-burmenska/

Our portfolio with the previous projects: https://docsend.com/view/fjrvjtyzgm7wgrkj

### Team Code Repos

- [DAOsign Github](https://github.com/DAOsign)

- [Eugene Fine (CIDT)](https://github.com/ConsiderItDone)

- [Ramil Amerzyanov](https://github.com/ramilexe)

- [Misha Kushka](https://github.com/kushkamisha)

- [Oleksandra Burmenska](https://github.com/burmenska)

### Team LinkedIn Profiles

- [Eugene Fine](https://www.linkedin.com/in/eugenefine/)

- [Ramil Amerzyanov](https://www.linkedin.com/in/ramil-amerzyanov/)

- [Misha Kushka](https://www.linkedin.com/in/mkushka/)

- [Oleksandra Burmenska](https://www.linkedin.com/in/oleksandra-burmenska/)

## Development Roadmap 

| Grant Milestones | Detail of work to be implemented to achieve milestone | Intended Outcome for Ecosystem/Users | Expected time required for delivery | Resource allocation |
|-------------------|--------------------------------------------------------|----------------------------------------|-------------------------------------|----------------------|
| Vechain Testnet Version | The ability to store proofs on the Vechain Testnet blockchain and verify them there. "Create an agreement" implementation; Assigning signers and observers; Implementation of Proof-of-Authority, Implementation of Proof-of-Signature, Implementation of Proof-of-Agreement. Early adopters program preparation |  Ability to choose different user verifications for Agreement signers and verify user profiles. | Q1-Q2 2024 | 20,000 |
| Incentivized Testnet version | Early Adopters Program launch; Online onboarding events; Feedback collecting; Roadmap adjustment | Adjusted roadmap based on Early Adopters' feedback | Q1-Q2 2024 | - |
| Mainnet version | Launching blockchain-stored and verified proofs version of DAOsign. Production support System resiliency; NFT-based Signer Authority Verification System | Publicly verifiable, flexible Signer Identity Verification System | Q2-Q3 2024 | 10,000 |


#### Community engagement

Twitter: https://twitter.com/dao_sign

LinkedIn: https://www.linkedin.com/company/daosign/

Discord: https://discord.gg/AwnhGFbT8Z

Telegram: https://t.me/DAOsign

Although we have not allocated funds for the social media, we have a great plan that we are following. We are actively maintaining our social networks, posting regular updates, guides, and will also soon be holding AMAs with our partners. More detailed statistics can be found here: https://docs.google.com/document/d/1Lo0XGODuihE3Ncn-8Wq30BeuH2XalzFrxI9uahY8Ad0/edit?usp=sharing. Also feel free to check our latest article with annual social media summary: https://www.linkedin.com/pulse/daosign-2023-numbers-social-media-edition-daosign-11axe%3FtrackingId=7ikItZPUMEgRYZjzloxwMw%253D%253D/?trackingId=7ikItZPUMEgRYZjzloxwMw%3D%3D

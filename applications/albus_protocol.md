# VeChain General Grant Application Template

## Project Overview 
- Project: Albus Protocol
- #1 DeFi Start-up in Switzerland (May 2023 - f6s.com Rating)
- Legal team Name: mFactory GmbH 
- Payment Address: USDC (ERC 20) payment address: 0x7C79d03F406B3a75C54c5F6e06688AC58cA45d3e

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview
- The Albus Protocol is a Compliance-as-a-Service on-chain infrastructure with Zero Knowledge proof and free of sign-up costs for all DeFi projects to enable them easily meet the requirements of the regulated crypto space.

- VeChain is perfect in our opinion because it already has a proven by many B2B customers supply chain solution. And, because supply chains are inextricably linked with DID applications as well as KYC/AML regulation, we are excited to make VeChain one of the first blockchains where Albus will be deployed.

- Sync2/Connex: Sync2 is a web application that allows users to access and manage their digital assets, while Connex is a standard interface to connect DApps with VeChainThor blockchain. Albus can integrate with these tools to extend its identity verification and compliance services to the VeChain network. DApps built on VeChain can use Albus' services for ZKP-based verification.

- Fee Delegation Protocol (VIP-191): Albus could leverage VeChain's Fee Delegation Protocol (VIP-191) to cover network transaction fees on behalf of users. This protocol allows a sponsor (in this case, Albus) to pay for transaction fees. This could help to provide a better user experience by removing the need for users to hold and spend VTHO for transactions, thus lowering the entry barrier.

- Multi-Task Transaction (MTT): VeChain's MTT feature allows bundling of multiple tasks into a single transaction. This could increase efficiency of Albus when dealing with complex compliance verifications that involve multiple steps or parties. A single MTT could include actions like creating a certificate request, updating user data, and validating compliance, thereby reducing the time and computational resources needed to complete these tasks separately.

### Project Details
> Mockups/designs of any UI components

Please see screenshots at our [website](https://albus.finance)

> API specifications of the core functionality

The developer and web SDK documentation will contain the API specification

> An overview of the technology stack to be used

We use:
- W3C standards for Verifiable Credentials and Verifiable Presentations
- zkSNARK Groth16 construction + BN128 (other curves can be used as well, e.g. BLS12-381) + Baby Jubjub Elliptic Curve (for optimal verification within circuits) + Poseidon hash function for generating and verifying Zero-Knowledge Proofs
- circom for building cryptographic circuits
- Sparse Merkle Tree for checking data integrity in Verifiable Credentials
- EdDSA + Poseidon hash function for signing Verifiable Credentials with the Issuer's signature and verifying the signature

> Documentation of core components, protocols, architecture, etc. to be deployed

Please see the documentation at [the Albus wiki](https://github.com/mfactory-lab/albus/wiki)

The architecture diagram, as well as other diagrams can be found at [the Albus diagrams page](https://github.com/mfactory-lab/albus/wiki/Albus-diagrams)

> PoC/MVP or other relevant prior work or research on the topic

Please see the documentation at [the Albus wiki](https://github.com/mfactory-lab/albus/wiki), and our [website](https://albus.finance)

### Ecosystem Fit

> Are there any other projects similar to yours? If so, how is your project different?

There are several on-chain KYC providers.
However, Albus has several differentiating factors and strong advantages as it uses Zero-Knowledge Proofs to ensure privacy of users' personal data, and also complies with KYC/AML regulations by storing such data on-chain in encrypted form, where it is available for potential requests of government agencies and cannot be deleted by the user.

## Team 

### Team members
- Alexander Ray - Founder, CEO
- Leonid Krassovitski - Co-Founder, CTO
- Sonny Wolfson - Co-Founder, CBDO


### Team Website
- https://albus.finance

### Team's experience
Proven successful track record
- [JPool.one](https://jpool.one/): a top-3 liquid staking pool on Solana 
- [Smart Validator Toolkit (SVT)](https://svt.one): an all-in-one validator cockpit that automates the processes of bootstrapping and maintaining Solana nodes
- [Staking Kiwi](https://staking.Kiwi): a Solana validator
- Projects for General Electric, Deutsche Bank, Swisscom

### Team Code Repos
https://github.com/mfactory-lab/albus

### Team LinkedIn Profiles
[Alexander Ray](https://www.linkedin.com/in/alex-a-ray/)

[Leonid Krassovitski](https://www.linkedin.com/in/leonid-krassovitski/)

[Sonny Wolfson](https://www.linkedin.com/in/sonny-wolfson/)


## Development Roadmap 

### Overview
| | Milestone 1 | Milestone 2 | Milestone 3 |
|-|-|-|-|
| Estimated Duration |                 30 d                |            15 d              |       15 d      |
| Full-time equivalent (FTE) | 2 | 1 | 3 |
| Cost (up to $ 30,000)|             $ 9,000               |          $ 6,000            |     $ 15,000    |


### Milestone 1 — Core functionality
| # | Deliverable | Specification |
|-|-|-|
| 1 | KYC verification | Conduct KYC verification of users via KYC providers (integration with existing KYC providers) |
| 2 | User data | Convert user data from KYC providers to Verifiable Credentials (VC) |
| 3 | VC and VP | Issue Verifiable Credentials (VC) and create Verifiable Presentations (VP) from VC (on-chain/NFT) |
| 4 | ZK Proofs | Generate ZK Proofs based on Verifiable Presentations (VP), verify ZK Proofs |
| 5 | Certificates | Issue Compliance Certificates (on-chain/NFT) |

### Milestone 2  —  Policies and certificates
| # | Deliverable | Specification |
|-|-|-|
| 1 | Policies | Create and manage policies (for DeFi business users) |
| 2 | Certificate verification | Verify Compliance Certificates through the Albus Protocol to proceed with transactions |

### Milestone 3  —  Web3 dApp and documentation
| # | Deliverable | Specification |
|-|-|-|
| 1 | Web3 dApp | Deploy web-based interface for DeFi users and  platforms |
| 2 | Documentation | Publish developer documentation |
| 3 | Web SDK | Deploy a web SDK for integrating the Albus Protocol |


## Community engagement
We plan to grow (and are already growing) the community through active participation in conferences (including speakers), and our own platforms (Discord, Twitter, LinkedIn)

Press releases:
https://albus.finance/#press

Social channels:

- Web: https://albus.finance 
- Twitter: https://twitter.com/AlbusProtocol  
- LinkedIn: https://www.linkedin.com/company/albus-protocol/ 

## Future Plans
- Onboard more vendors and users
- Implement cross-chain capabilities
- Increase coverage by including additional sectors of real-world economy
- Become a #1 Compliance-as-a-Service solution for DeFi projects within the next 3 years

## Additional Information 
Stage
- Grant secured from Solana Foundation
- Preview released in May: https://github.com/mfactory-lab/albus 
- MVP to be released in late Summer 2023
- Soft commitments signed by multiple partners

Key backers
- Solana Foundation
- BNB Chain 

Enabler partners
- SumSub (KYC provider)
- IDNow (KYC provider)
- Chainalysis (AML provider)
- Mob.ID (SSI provider)
- CurioInvest (RWA Tokenizator)
- Marinade (DeFi liquid staking Protocol)
- SelTech Group (Tanzanian Fintech innovator)
- Hubble Protocol (DeFi Protocol on Solana)

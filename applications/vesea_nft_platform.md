# VeChain General Grant Application

## Project Overview 

- **Project:** VeSea NFT Utility Platform
- **Team Name:** VeSea 
- **Payment Address:** 0x9D152D78B05f31EA6979061d432110c8664cA1a7

## `Overview`
**Description**
VeSea NFT Marketplace, Launchpad and utility platform is being created to enable the creation, discovery and transacting of VIP-181 tokens within the VeChainThor ecosystem, and to then empower those creators and their NFT holders with day-1 utility of those same tokens via modular, composable smartcontracts.   

**Reasoning**
As we all know, NFTs have become a prominent vehicle for elevating the web3 discussion and general activity across all of blockchain. Our team saw that growth happening across all major chains while our most-invested ecosystem remained stagnant for retail/community participants. Seeing that stagnation on VeChainThor's user-facing interactions was when and why we sought to bring that energy, those conversations, all of the engagement and creativity (both artistic and builder) to VeChain.

**Features and Enhancement**
- Full wallet support
- Connex
- MTT
- VIP-180 management
- VIP-181 management
- Fee delegation
- Forcible Transaction Dependency (*coming*)
- Transaction Lifecycle Control (*coming*)

## `Designs of UI Components` 
_Can be viewed on our site_ ([VeSea](https://vesea.io/))

 ### Landing Page ![Landing](https://s3.us-east-2.amazonaws.com/vesea.io/grant/Homepage.png)
    
 ### Collection Pages
  * Collections
    ![Collections](https://s3.us-east-2.amazonaws.com/vesea.io/grant/Collections.png)
  
  * Collections Market
    ![Collection Market](https://s3.us-east-2.amazonaws.com/vesea.io/grant/Collection_Page.png)
 
  * Collections Mint
    ![Collection Mint](https://s3.us-east-2.amazonaws.com/vesea.io/grant/Launchpad.png)
    
  * NFT Modal
    ![NFT Modal](https://s3.us-east-2.amazonaws.com/vesea.io/grant/NFT_Modal.png)
    
  * Launchpad
    ![Launchpad](https://s3.us-east-2.amazonaws.com/vesea.io/grant/Launchpad.png)
    
 ### Profile Pages
  * Profile Creation
    ![User Creation](https://s3.us-east-2.amazonaws.com/vesea.io/grant/Profile_Creation.png)

  * User Notifications
    ![User Notifications](https://s3.us-east-2.amazonaws.com/vesea.io/grant/Notifications.png)

  * User Settings
    ![User Settings](https://s3.us-east-2.amazonaws.com/vesea.io/grant/Profile_Management.png)
   
 ### Functions
  * VIP-180 Management
    ![VIP-180 Management](https://s3.us-east-2.amazonaws.com/vesea.io/grant/VIP180_Transfers.png)

  * On-Chain Messenger
    ![Messenger](https://s3.us-east-2.amazonaws.com/vesea.io/grant/Messenger.png)

## `Tech Stack` 
| Bridge Component | Stack |
| :-: | :-: |
| Storage | IPFS, Arweave |
| Smart Contracts | Solidity |
| Backend | TypeScript |
| Frontend | React (JSX, TypeScript) |
| Architecture | AWS |


## `Ecosystem Fit` 
Are there any other projects similar to yours? If so, how is your project different?
Yes, we are one of three multi-collection NFT markets, but have emerged as the leader in transacted volume YTD by an order of magnitude due to our community engagement, launchpad program and the open implementation of our setup enabling other ecosystem builder and tools. 
- NFT Marketplaces:
  - [VeSea](https://vesea.io/)
  - [World of V](https://marketplace.worldofv.art/)
  - [BlackVeMarket](https://blackvemarket.com/)

- [Recent Stats](https://www.vesea.io/resources/stats)

We aim to continue with an approach of a curated platform to maintain trust within the ecosystem, and as project growth expands to then create an ecosystem for those vetted projects to deliver functionality more readily using our multi-collection utility contracts. We've detailed our plans going forward recently on Medium, discussing our platform direction [here](https://medium.com/@VeSea/vesea-marketplace-launchpad-utility-platform-62803313808c) and the lifeblood of that ecosystem ($VSEA) [here](https://medium.com/@VeSea/vsea-vechains-nft-utility-era-c26537d8fa8f).

Long-term, the hope is to make VeChain a destination for NFT projects across all of blockchain by leveraging XP Network's NFT Bridge, a superior chain-interaction experience and instant NFT utility.

## `Team` 

### Team members

- Product Manager: Bread (https://github.com/Bread-VeSea) 
- Full-stack Dev: Emmet (https://github.com/EmmetA) 
- Full-Stack Dev: He-Man (via PM)
- Front-End Dev: Shrimp (via PM) 

### Team Website

- https://vesea.io

### Team's experience

The team is comprised of full-time IT professionals with over 60 years of experience from industries both inside and out of the web3 space and with entrepreneurial experience growing 4 separate companies. Specific details can be given via PM if desired.

### Team Code Repo

https://github.com/VeSeaOfficial

### Team LinkedIn Profiles

Provided via PM, if desired

## `Development Roadmap`   

### Milestone Details

#### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3 | 
| - | - |- | - |
| Estimated Duration | Done | Done | 60 d |
| Full-time equivalent (FTE) | 2 | 2 | 2 |
| Cost    | 10,000 USD | 10,000 USD | 10,000 USD  |

Estimates are based on the part-time participation of 4 separate developers (~4hr/d/person, x6d/w) plus platform infrastructure and management costs over the span of the 10 months we've been in operation (launch Oct 8th, 2021).

#### `Mandatory` — License, Documentation and Unit Tests
| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | Apache 2.0 |
| 0b,c. | Documentation, Testing | A github with our contracts and unit tests will be provided on request |

#### `Milestone 1` — Smartcontracts, Backend & UI

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Smart Contracts | We will develop VIP-181-supporting smart contracts that will allow for:<br>1. Listing/purchasing<br>2. Bidding <br>3. Sending/Receiving<br>4. Escrowing<br>5. Setting of minimum offers<br> |
| 2 | Frontend | We will create a dApp that:<br>1. Displays all supported NFTs of a user<br> 2. Supports all foundation wallets |
| 3 | Backend | Implement local database to aggregate:<br>1. On-chain data<br>2. IPFS metadata<br>3. Local information |

#### `Milestone 2` — Features

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Smart Contracts | Implement:<br>1. On-chain profiles (sensitive info local)<br>2. Multi-wallet method access for assisted NFT launches<br>3. Modular burn event for VIP-181 contracts<br>4. Consolidated marketplace contract<br>5. Implement leveraged collection-wide offers for single VIP-181 contracts|
| 2 | Backend | 1. Design, build of indexer<br>2. Implementation of fee delegation infrastructure|
| 3 | Frontend | Implementation of:<br>1. User Profiles <br> 2. On-Chain Messenger <br> 3. VeSea Arcade for multi-collection, game-like mechanics|

#### `Milestone 3` — Smartcontracts, Backend & UI v2

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Smart Contracts | We will develop smart contracts that will:<br>1. Leverage VIP-180 tokens<br>2. Allow for NFTs to "battle"<br>3. Allow for VIP-181 staking to earn VIP-180 tokens<br>4. Allow for dynamic fee calculations based on NFT holdings|
| 2 | Backend | Implementation of:<br>1. Indexer<br>2. Open API for ecosystem builders|
| 3 | Frontend | Implementation of:<br>1. VIP-180 Transfers<br> 2. On-Chain Messenger<br> 3. Create dashboards to reflect on-chain information for sales, staking and general transactions|

## `Community engagement`    

We have already established ourselves as a trusted platform within the VeChain ecosystem, working to partner with individual collections to either launch or become their secondary market alongside integrations with various other VeChain dApps such as VeChainStats (block explorer), VeChain.Energy (fee delegation) and NFT launches for both Hacken (Ukraine Relief) and VeRocket (Utility NFT launch).

Along with project collaborations, we've also had a strong presence on Twitter, in Twitter Spaces, have 2 VeChain Brand Ambassadors within the team and have been feature on VeChain Thorsdays and on the Sunny's Community Hangout as a leader in the space.

#### Socials
- Twitter: https://twitter.com/VeSeaOfficial
- Medium: https://medium.com/@VeSea
- Discord: https://discord.gg/vesea

## `Future Plans` 

[VeSea: Marketplace, Launchpad, Utility Platform](https://medium.com/@VeSea/vesea-marketplace-launchpad-utility-platform-62803313808c)
[$VSEA: VeChain's NFT Utility Era](https://medium.com/@VeSea/vsea-vechains-nft-utility-era-c26537d8fa8f)

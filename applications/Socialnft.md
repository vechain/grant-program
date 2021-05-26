# VeChain General Grant Application Template

## Project Overview 

- Project: Socialnft
- Team Name: EditorAi 
- Payment Address: 0x4126aC8a3813068ece67b47489e2aEA4B66226D8  USDT (ERC 20) payment address. 

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

An NFT platform supporting VeChain.
It supports celebrities on Social Media platforms to convert posts into NFTs with one click, hence enriching the ecosystem of VeChain NFT.

Cheap VTHO compared to Ethereum Gas fee. Hope to cut the costs to 1/1000 by creating the platform on VeChain with NFT trading and payment settlement.

Use Fee delegation to Pay for the creator using the platform when minting the NFTs, that’s the coolest feature we are excited about using VeChain.
We hope to ease the steps of purchasing and selling by using the MTT feature (approve, transfer in one transaction using multi-clauses).


### Project Details

#### **Mockups/designs of any UI components**

- https://lanhuapp.com/url/FsAGx

#### **API specifications of the core functionality**

- Accounts management
- Post(Items) management
- Wallet management
- Transaction management

#### **An overview of the technology stack to be used**

- API: Nodejs + Express
- Web: React + Redux(create-react-app)

#### **Documentation of core components, protocols, architecture, etc. to be deployed**

The core component is to support mint NFT tokens for user’s instagram posts. And everyone can buy & sell instagram NFT on the platform. And we use third part payment APIs to power our fintech application. 

The system is comprised of following parts:

- NFT (VIP-181) is minted and traded on the VeChain Thor Blockchain.
- User Wallet is using the Vechain Sync wallet.
- NodeJS server is responsible for marketplace display and interacting with users.
- Posts are fetched from Instagram.
- Backend is of Monolithic architecture.

![image](https://ipfs.io/ipfs/bafkreibnpzq5ano4fkjaampday5yivdtcwbgnjyqnkeh33h26tp3biz2qe)

- PoC/MVP or other relevant prior work or research on the topic.

Our previous developed NFT market is the earliest Chinese version of Cryptoart Market based on ERC721 launched in 2020. The platform so far has almost 1000 artist with 500+ artwork uploaded. More than 300 artworks were sold at the average prive above 1 ETH. We are fully experience with creating NFT market.


### Ecosystem Fit

Per our research, currently on VeChain there is only VIM-world as an NFT platform, but ours is much different as we convert social media posts directly into NFTs, thus we have more contents.

On Ethereum, we have a benchmark v.cent.co converts twitter tweets to NFT. We convert instagram posts to NFT. And they are not on VeChain yet.

## Team 

### Team members

#### **Name of team leader**

- Pablo

#### **Names of team members**

- Aiboo
- Joe
- Maco


### Team Website

- Under construction, expected to be launched on June.

### Team's experience

- Successful NFT market development experience on Ethereum.

### Team Code Repos

- https://github.com/editorai/socialnft-web

- https://github.com/editorai/socialnft-api

- https://github.com/editorai/marshmallow-v1


### Team LinkedIn Profiles

## Development Roadmap 

#### **Overview**

|  | Milestone 1 | Milestone 2 | Total |
| - | - |- | - |
| Estimated Duration | 30 d | 30 d | 60 d |
| Full-time equivalent (FTE) | 4 | 4 | 8 |
| Cost (up to $ 30,000) | $ 15,000 | $ 15,000 | $ 30,000|

<br/>

#### **Milestone 1 — Prototype**

| Number | Deliverable | Specification |
|-|-|-|
| 1 | prototype | We will develop prototype that demonstrate the process of converting instagram posts to NFT and making it tradable on our platform. The workload includes detailed product and UI design, connecting and testing facebook API, setting up filecoin and ipfs storage, all non-blockchain frontend and backend realization|

<br/>

#### **Milestone 2  —  Smart Contract & integration on Vechain**

|  | Milestone 1 | Milestone 2 |
| - | - |- |
| 1 | Frontend | We will finish the development of frontend part that connects with sync wallet to mint and transfer NFT |
| 2 | Backend | Establish the wallet service to receive assets on Vechain |
| 3 | Smart Contract | NFT smart contract on Vechain |

<br/>

#### Community engagement

As part of the Program, we require that you produce and publish at least one article/tutorial (e.g., on Medium). It should explain your work done as part of the grant.

## Future Plans

- Integrating more social network

- Issue social token

- Offer to earn mode

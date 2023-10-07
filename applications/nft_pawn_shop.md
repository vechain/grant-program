# NFT Pawn Shop Grant Application

## Project Overview 

- Project: NFT Pawn Shop
- Team Name: Berzan Bozhan 
- Payment Address: `0x2Fea522d64a208281F5FCA7c83b3977b37c90Cd6`


### Overview
My project is NFT Pawn Shop.<br>
It is a decentralized application that allows VeChain users to borrow money <br>
using their NFTs as collateral and earn interest by becoming a pawn broker.<br>
Other projects will be able to integrate their dApps with it and provide the same services.<br>
I believe that one day this project will be a standard for the entire VeChain ecosystem and each dApp will integrate it.

I'm pretty confident that I can build this project in a way that I will be proud of. <br>
Building the project as safe & trustless won't be possible without a blockchain like VeChain.<br> 
I hope this project will help VeChain community to access money without selling their NFTs and earn interest by lending money.

### Project Details

- NFT Pawn Shop is consisted of servers (backend server) and clients (users of the frontend).
- Clients interact with the smart contract, and fetch data from servers.
- Servers connect to VeChain nodes to fetch data from the smart contract.
- Servers also connect to 3rd party NFT marketplaces for price data.
- [Rust](https://www.rust-lang.org/) will be used for the backend server.
- [TypeScript](https://www.typescriptlang.org/), [Svelte](https://svelte.dev/) and [TailwindCSS](https://tailwindcss.com/) will be used for frontend.
- The backend server will have a custom in-memory cache.
- A custom design system will be used for the website.
- Both the backend server and the frontend will be published as a [Docker](https://www.docker.com/) image.
- Any NFT Marketplace or dApp will be able to integrate NFT Pawn Shop.


### Ecosystem Fit
There are a few NFT marketplaces like VeSea, OceanEx, World of V, etc.<br>
But none of them offer borrowing/lending services like NFT Pawn Shop will do.<br>
Also those NFT marketplaces will be able to integrate their dApps with NFT Pawn Shop using our documentation.<br>
So no matter what dApp VeChain users use they will be able to access the same services everywhere.

## Team 

### Team members
I am the solo developer who will build NFT Pawn Shop.

- Berzan Bozhan

### Team Website
I currently don't have a personal website, but my GitHub profile is below.
- https://github.com/BerzanXYZ/

### Team's experience

I have been programming for around 4 years, though I've been late to create a GitHub profile.<br>
I've developed desktop applications, a few simple games, CLI tools, simple dApps, websites, etc.<br>
I worked for a few crypto projects last year but then I took a break.<br>
I've been improving my knowledge about various concepts ever since.<br>
I am confident that I can build this project as expected.<br>
Some projects I've been developing recently are below.

### Team Code Repos

- https://github.com/BerzanXYZ/cosmwasm-name-system-contract
- https://github.com/BerzanXYZ/aptos-social-network-interface
- https://github.com/BerzanXYZ/aptos-dictionary-interface
- https://github.com/BerzanXYZ/aptos-social-network-contract
- https://github.com/BerzanXYZ/aptos-dictionary-contract

### Team LinkedIn Profiles
I don't have/use a LinkedIn profile.

## Development Roadmap 

#### Overview

|  | Milestone 1 | Milestone 2 | Total |
| - | - |- | - |
| Estimated Duration | 50 d | 40 d | 90 d |
| Full-time equivalent (FTE) | 1 | 1 | 1 |
| Cost (up to $ 30,000) | $ 9,500 | $ 8,000 | $ 17,500|

#### Milestone 1 — Smart Contract & Backend

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | MIT |
| 0b.| Development Environment | I will create [Dev Containers](https://containers.dev/) to make it easy to set up development environments. |
| 1a. | Smart Contract: Development | I will develop the smart contract of NFT Pawn Shop. <br> It will include all the features like borrowing VET tokens using NFTs as collateral, lending VET tokens to earn interest, etc. |
| 1b. | Smart Contract: Testing | The smart contract will have proper unit-test coverage to ensure functionality and robustness. |
| 1c. | Smart Contract: Documentation | I will build a documentation website both for contributing and interacting with the smart contract. |
| 2a | Backend: Development | I will develop a backend server for NFT Pawn Shop since VeChain nodes should not be kept busy.<br> It will be written in Rust language and use a cache to offer low latency. <br> Third party NFT marketplaces will be integrated for price data, etc. |
| 2b. | Backend: Testing | The backend server will have proper unit-test coverage to ensure functionality and robustness. |
| 2c. | Backend: Documentation | I will build a documentation website both for contributing and interacting with the backend server. |
| 2d. | Backend: Docker Image | I will publish a Docker image for the backend server. |

#### Milestone 2  — Client SDK, Wallet Adapter & Frontend
| Number | Deliverable | Specification |
|-|-|-|
| 1a | Client SDK: Development | I will develop client SDK for NFT Pawn Shop and publish it to [`NPM`](https://www.npmjs.com/).<br> It will make it easy to interact with the backend server without keeping VeChain nodes busy. |
| 1b | Client SDK: Testing | The client SDK will have proper unit-test coverage to ensure functionality and robustness.  |
| 1c | Client SDK: Documentation | I will build a documentation website both for contributing and using the client SDK. |
| 2a | Wallet Adapter: Development | I will develop a wallet adapter for VeChain using [Svelte](https://svelte.dev/) framework and publish it to [`NPM`](https://www.npmjs.com/). <br> It will support all popular VeChain wallets. |
| 2b | Wallet Adapter: Testing | The wallet adapter will have proper unit-test coverage to ensure functionality and robustness.  |
| 2c | Wallet Adapter: Documentation | I will build a documentation website both for contributing and using the wallet adapter. |
| 3a | Frontend: Development | I will develop a frontend for NFT Pawn Shop using [SvelteKit](https://kit.svelte.dev/) & [TailwindCSS](https://tailwindcss.com/).<br> It will use the client SDK, the wallet adapter and the backend server.<br> I will use best practices to provide a good user experience. |
| 3b | Frontend: Testing | The frontend will have proper unit-test coverage to ensure functionality and robustness.  |
| 3c | Frontend: Documentation | I will build a documentation website both for contributing and using the frontend. |
| 3d. | Frontend: Docker Image | I will publish a Docker image for the frontend. |
| 4a | Integration With Other dApps | As the client SDK only supports Svelte, I will implement React and Vue support for the client SDK. <br> To make it easy to integrate any dApp with NFT Pawn Shop, I will build a documentation website for integrations.<br> It will include tutorials for frontend frameworks like React, Vue and Svelte. |


#### Community engagement

I will create a Medium profile for NFT Pawn Shop and publish articles during the development.<br>
I will also create a Twitter profile for NFT Pawn Shop to promote the project and VeChain.

## Future Plans

My goal is that each part of the project will be owned and maintained by VeChain community.<br>
A good documentation will make it possible for any dApp to integrate NFT Pawn Shop.<br>
Hopefully, on chain activities will increase because of NFT Pawn Shop.

## Additional Information 

I haven't started to develop NFT Pawn Shop yet.<br>
The only way for me to start building this project is getting a grant, because NFT Pawn Shop will not charge any fees.
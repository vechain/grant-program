# VeChain General Grant Application Template

## Project Overview 

- Project: VeTools - VeChain VSCode Toolkit
- Team Name: Magnus Ekström
- Payment Address: 0xf7e009D8E3F012286415aE576Fcaa50c38bAFCb7


### Overview

We propose the development of VeTools, a potent and comprehensive VSCode Extension designed to revolutionize the development process on the VeChain Thor Blockchain network. 
The core idea behind the project is to simplify the process of writing, compiling, and debugging smart contracts on VeChain. Our vision is to make this toolkit seamlessly integrated into VSCode, 
thereby providing extensive Solidity debugging support. By leveraging VSCode's standard debugging features, such as breakpoints, variables, and watches, we aim to offer developers a familiar and 
intuitive set of tools to build dApps on VeChain.

My interest in creating this project within the VeChain Ecosystem is driven by the potential I see in VeChain's infrastructure. In my past year of being involved in the ecosystem, 
I acknowledge VeChain's scalability, security, and well-structured governance model as an excellent platform for nurturing a wide range of applications and businesses. 
I believe our proposed tool could empower developers to more efficiently utilize VeChain's capabilities, contributing to the ecosystem's growth and diversity.

The proposed toolkit, VeTools, is envisioned to function out-of-the-box, delivering a preconfigured set of tools to expedite every phase of Smart Contract development, from writing to compiling, 
deploying, and debugging. As an all-inclusive solution, VeTools seeks to provide built-in integration with Thor, presenting a frictionless edit-build-debug-and-deploy environment that assures 
consistency across mainnet, testnet, and local nodes.

One of the key features in our proposal is the built-in Solidity Debugger. This tool will enable developers to debug Solidity contracts easily against a local Thor node. 
I firmly believe that VeTools could serve as a catalyst in empowering developers, which we anticipate will result in a surge in the number and quality of dApps on the VeChainThor network. 
As this project is still in its conception phase, we eagerly anticipate the opportunity to bring this vision to life and contribute to the VeChain ecosystem


### Project Details

My final aim is to provide a fully-functioning VSCode extension providing the following features:
- creating quick project boilerplates (similar to create-react-app, but on VSCode)
- compiling contracts
- deploying contracts to mainnet/testnet/local node
- debugging contracts via VSCode's native debugger
- creation & managemtn of local blockchain instances
- creation & management of wallets
- transfer of assets like VET/VTHO between wallets
- interactive blockchain exploration

... from within VSCode

### Ecosystem Fit

Currently there is no such toolkit available on VeChain. My belief is that this will greatly help developers build and ship dApps quickly without leaving the comfort of their favorite editor

## Team 

### Team members

- Magnus Ekström

### Team's experience

I'm a CS degree holder with 7+ years of experience. I have been active in the blockchain space since 2018 and have been continuously building on major chains and networks, having built all sorts of dApps from liquid staking protocols to cross-chain protocols. Last year, I was introduced to VeChain and I have not looked back since.

### Team Code Repos

- https://github.com/hazelcaus

### Team LinkedIn Profiles

- https://www.linkedin.com/in/magnus-ekstr%C3%B6m-46b993278/


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
| Estimated Duration | 15 d | 15 d | 45 d |
| Full-time equivalent (FTE) | 1 | 1 | 1 |
| Cost (up to $ 30,000) | $ 10,000 | $ 10,000 | $ 10,000|

#### Milestone 1 — Foundational Development & Compiler Integration

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | 	GNU Lesser General Public License v3.0 (GPLv3)  |
| 1 | Boilerplate generation code | includes defining standard project structure, configuration files, and commonly used contract templates  |
| 2 | Integration of the Solidity compiler | Building the compiler module that accepts the contract code, compiles it, and returns bytecode and ABI |
| 3 | Comprehensive Unit Testing | Establish the foundation for a robust and reliable codebase |

#### Milestone 2  —  Advanced Deployment and Debugging Environment 

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | 	GNU Lesser General Public License v3.0 (GPLv3)  |
| 1 | Deployment module | Writing scripts that will deploy compiled contracts to VeChain's mainnet, testnet, or a local node. This includes managing private keys securely and handling deployment parameters |
| 2 | Integration of debugging tool | Development of a module that interfaces with VSCode's native debugger and handles Solidity-specific debugging needs. This module will also provide mapping between compiled bytecode and source code for an efficient debugging experience |
| 3 | Local blockchain instance manager | Build a feature that can initiate, pause, resume, or terminate local Thor nodes, with the option to configure the node parameters. |

#### Milestone 3  —  Wallet Operations and Blockchain Interactions

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | 	GNU Lesser General Public License v3.0 (GPLv3)  |
| 1 | Wallet manager | Building a tool for creating and managing VeChain wallets securely. This includes handling of public-private key pairs, and encryption for secure storage  |
| 2 | Asset transfer module | Develop a feature to facilitate the transfer of VET/VTHO between wallets, including transaction signing and sending |
| 3 | Blockchain explorer | Build an interactive explorer that allows developers to browse blocks, transactions, and accounts on the VeChain blockchain. This module will also facilitate contract interaction, allowing function calls and state variable queries |

#### Community engagement

I will write a Medium article after our initial deployment detailing usage instructions. I also plan to include a simplistic demo to showcase the framekwork by "show-by-example" method.

## Future Plans

My main focus is improving the developer experience. I've been fascinated with VeChain overall and excited for its development, so I have a bunch of other ideas in the pipeline. I will continue to provide long-term maintenance for this project (including replying to GitHub issues). 

## Additional Information 

Possible additional information to include:
- What work has been done so far? Initial stages of implementation
- Are there any teams who have already contributed (financially) to the project? No
- Have you applied for other grants so far? No

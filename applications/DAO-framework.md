# VeChain DAO Framework Grant Application

## Project Overview 

- Project: DAO Framework
- Team Name: SayNode Operations AG
- Payment Address: 0x989A38EDEbd2Bd80d4949a9F7462C93FA8055876


### Overview

We would like to provide a solution for creating a Decentralized Autonomous Organization (DAO) on VeChain in a simpler way. SayNode Operations is creating a DAO using the VeChain network and we would like to create a simpler way for other future projects and other developers working on VeChain to launch a DAO. We intend to create a library with all the functions needed for the DAO development. This library will allow developers to not spend hours on developing each functionality themselves but doing it in a shorter and easier way by using the DAO library created by us.

The main goal of this project is to build a solution to simplify the developers work and eliminate the existing hurdles. 


### Project Details

We have divided the project into 5 sub-steps. 
Create a library which will be able to:
- import wallets and connect to a VeChain node.
- handle proposals, voting and queue/execute functions of the DAO.
- grant and revoke governance roles (for example give proposer roles to everybody, executer role to the governance contract address and revoke the TimeLock admin role from the contract deployer).
- wrap and unwrap the VIP180 token of the DAO (in case it was not made with the standard ERC20Votes extension).
- doing all this making use of the OpenZeppelin standard DAO smart contracts, allowing for the creation of safe and tested DAOs.


The individual milestones and their duration can be viewed in detail below. 

### Ecosystem Fit

Developers who want to create a DAO on VeChain will need to add additional support to make all the connections to VeChain wallets, to grant and revoke roles, handle proposals and wrap the token the moment you vote, and unwrap after (to take snapshots before each vote). In order to simplify this process we will create this library which will have all these functionalities ready to use for the developers. DAOs are booming on other chains but sadly there are not many DAOs on VeChain. We aim to make it easier to create a DAO on VeChain.


## Team 

### Team members

- Renato Schär
- Werner Liechti
- Yann Marti
- Paula Amstutz
- João Morais
- Riccardo Mazzucchelli
- Francesco Romeo
- Simon Heer

### Team Website

- https://saynode.ch/

### Team's experience

The SayNode Operations team has already implemented several projects for the company, including for VeChain. Besides the token migration of Dohrnii Foundation https://dohrnii.io/ from Ethereum to VeChain, a first project directly for VeChain has already been implemented. Further, a grant has already been awarded by VeChain for the Dev-Thorkit-Dart see here: https://github.com/VeChain/grant-program/pull/51. Besides, a first Flutter App was developed, which was accepted by the Apple Store as well as the Android Store and can be found here: https://github.com/SayNode/342.

Renato Schär and Werner Liechti are CTOs of the Dohrnii DAO and CEO and COO of SayNode Operations. The Dohrnii project is a DAO solution with a native token DHN on Ethereum, VeChain and Binance. The technical implementation of the Dohrnii project is mainly done by SayNode Operations (https://dohrnii.io/). Both have a computer science background and a degree from a Swiss university.

Yann Marti is a Flutter Developer at SayNode Operations. He is an absolute specialist and does all frontend work for the Vidaia app as well as for Dohrnii. Likewise, he created the frontend for the already existing app (https://github.com/SayNode/342). For the already guaranteed grant of VeChain he also takes over a large part of the development. He is also studying Computer Science at the University of Bern. 

Paula and João are blockchain developers and have contributed heavily to the implementation of Dohrnii. They are and have also both been involved in SayNode Operations' other projects. Paula has a Bachelor's degree in IT Security and a Master's degree in Cryptography, Data Security and Blockchain and previous work experience. João has a Master's degree in Electrical and Computer Engineering and has worked as a Software Developer at Siemens Logistics. From May, Paula and João were joined by Riccardo Mazzucchelli who also has a background as a developer and had his own company in the crypto field. 

Francesco Romeo is a FullStack Developer and has a university degree in Computer Engineering. He has several years of experience as a developer in different companies and accompanied as CTO and Founder the startup BuyTime. The last years he worked as a FullStack Developer at the University of Applied Sciences in Bern. 

Simon Heer has worked several years in B2B Sales for RedHat and VmWare as well as in IT Risk and Compliance at AXA Insurance. He has a Master in Digital Business and Innovation and he is responsible for the business aspects of the products. 


### Team Code Repos

- https://github.com/SayNode  A few repositories are private because of confidentiality agreements
- https://github.com/RsTs23
- https://github.com/wernerliechti
- https://github.com/Dohrnii-Foundation
- https://github.com/YannMarti
- https://github.com/paulaamstutz

### Team LinkedIn Profiles

- https://www.linkedin.com/in/renato-sch%C3%A4r-8a9a19a5/
- https://www.linkedin.com/in/werner-liechti-568b19213/
- https://www.linkedin.com/in/paula-amstutz/
- https://www.linkedin.com/in/joaogmorais/
- https://www.linkedin.com/in/francesco-romeo-2867083b/
- https://www.linkedin.com/in/riccardo-mazzucchelli/
- https://www.linkedin.com/in/simon-heer-202866110/


## Development Roadmap 

### Roadmap for our dApp Application

#### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3  | Total |
| - | - | - | - | - |
| Estimated Duration | 15 d | 30 d | 20 d | 65 d |
| Full-time equivalent (FTE) | 0.5 | 2 | 1 | 3.5 |
| Cost (up to $ 30,000) | $ 3,500 | $ 14,000 | $ 7,000 | $ 24,500 |

#### Milestone 1 — DAO Smart Contract Integration

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | GNU Lesser General Public License v3.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial. |
| 1 | OpenZeppelin Smart Contracts Integration | Importing and integrating Governor, Governance TimeLock Smart Contract from OpenZeppelin. |
| 2 | Wrap/unwrap token | wrap and unwrap the ERC20 token of the DAO (in case it was not made with the standard ERC20Votes extension) in order to wrap the token the moment you vote, and unwrap after (to take snapshots before each vote). This is a simplification of the current method which requires somebody to already have wrapped tokens before a proposal is created.  |
| 3 | Changeable Contract | This contract will be governed and is the contract that the user wants to be changed. An example will be given in the project.|


#### Milestone 2  — DAO Library

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | GNU Lesser General Public License v3.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial. |
| 1 | Basic.py | We will import the wallet and connect it to the VeChain Network. |
| 2 | DAO.py | The library will enable proposal, voting and queue/execute functions for the DAO. |
| 3 | Roles.py | It will be possible to grant propose role to everybody, executor role to the governance contract address and revokes the TimeLock admin role from the contract deployer (so that he no longer controls the DAO in any way). |



#### Milestone 3  —  Deployment and running tests

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | GNU Lesser General Public License v3.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial. |
| 1 | Deployment | The contracts will be deployed on VeChain Network. |
| 2 | Test | The library will be tested to make sure its functionalities are all running. |




#### Community engagement

After the project is completed, an article will be created for Medium to inform developers and companies about the new possibilities. Also, SayNode Operations channels will be used to inform the community. Specifically, a blog post will be written on the website and a post will be made on LinkedIn. Also a documentation will be created that gives information about the handling and functionalities. 
 

## Future Plans

We will be able to create a DAO using this library and then use it every time we will be asked to create a DAO. In the future we might want to create an even easier interface that allows users to create DAOs with minimal to no coding experience based on this library. 

## Additional Information 

- What work has been done so far?

The planning of the project is all done, smart contracts integration and DAO.py, Roles.py and wToken are nearly finished. Some of the missing parts for a successful release is the creation of a connection with the wallet on the VeChain network, deployment of contracts and testing the library.

- Are there any teams who have already contributed (financially) to the project?

The project has not received any direct investment from other resources and is managed solely by SayNode Operations. 

- Have you applied for other grants so far?
No grant has yet been requested for this specific project. A grant has already been approved for a VeChain project with a different use case as mentioned above, see https://github.com/VeChain/grant-program/pull/51
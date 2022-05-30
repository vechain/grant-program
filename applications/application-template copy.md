# VeChain VeSayNodeV2 application

## Project Overview 

- Project: VeSayNodeV2
- Team Name: SayNode Operations AG
- Payment Address: 0x989A38EDEbd2Bd80d4949a9F7462C93FA8055876

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

This is the expansion of the V1 of our service. Three sub-steps are required for the implementation of the expansion. Our first version will be extended by an IPFS to ensure scalable and distributed storage. This means that developers no longer have to worry about their own IPFS nodes, but can interact with a link via an API provided by us. This also means that developers only have to pay how much they really need. For this we will integrate a wallet and a card payment system. 
Based on the previous grant request, we will work with a similar solution as Infura for scaling. In doing so, we will use snapshots to periodically update the current state of the blockchain. After the go-live, we will operate and maintain the solution commercially. 


### Project Details

In the milestones below the actual sub-steps and the required time are written down in more detail. 

The project is divided into three milestones. For each of them, we have created sub-steps with a more comprehensive explanation in the Milestones chapter.

1) IPFS gateway: We will extend our product with an IPFS API and dedicated gateway, enabling users to connect their application to distributed storage. Documentation and tutorials will be provided. 

2) Performance and scalability upgrades: We will ensure the scalability of the solution by creating a snapshot solution similar to the one Infura uses. 

3) Launch, operating and marketing costs: We will launch the service to the public and provide users with different plans that best fit their needs. The service will be maintained directly by SayNode Operations and will again include documentation and tutorials. To create an initial user base different marketing approaches will be chosen including payed ones. 

### Ecosystem Fit

Developers who want to interact with VeChain the way they are used to need a Web3 gear, which means scope and effort that developers may not want to take. We want to eliminate this barrier and give developers an easy way to program for VeChain through a solution they already know from other projects. We are taking on a role similar to what infura is doing for Ethereum and hope to provide a solution to developers with the new capabilities that will ultimately grow the entire Vechain ecosystem. 

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

The SayNode Operations team has already implemented several projects for the company, including for Vechain. Besides the token migration of Dohrnii Foundation https://dohrnii.io/ from Ethereum to Vechain, a first project directly for Vechain has already been implemented. Further, a grant has already been awarded by VeChain for the Dev-Thorkit-Dart see here: https://github.com/vechain/grant-program/pull/51, the implementation of the project is still ongoing. Besides, a first Flutter App was developed, which was accepted by the Apple Store as well as the Android Store and can be found here: https://github.com/SayNode/342.

Renato Schär and Werner Liechti are CTO of Dhornii Foundation and CEO and COO of SayNode Operations. The Dhornii project is a DAO solution with a native token DHN on Ethereum, VeChain and Binance. The technical implementation of the Dhornii project is mainly done by SayNode Operations (https://dohrnii.io/). Both have a computer science background and a degree from a Swiss university. They are also part of the new Draper University and VeChain Fellowship program with a new Product Vidaia (not live yet), which is also developed on VeChain

Yann Marti is a Flutter Developer at SayNode Operations. He is an absolute specialist and does all frontend work for the Vidaia app as well as for Dhornii. Likewise, he created the frontend for the already existing app (https://github.com/SayNode/342). For the already guaranteed grant of VeChain he also takes over a large part of the development. He is also studying Computer Science at the University of Bern. 

Paula and João are blockchain developers and have contributed heavily to the implementation of Dhornii. They are and have also both been involved in SayNode Operations' other projects. Paula has a Bachelor's degree in IT Security and a Master's degree in Cryptography, Data Security and Blockchain and previous work experience. João has a Master's degree in Electrical and Computer Engineering and has worked as a Software Developer at Siemens Logistics. From May, Paula and João were joined by Riccardo Mazzucchelli who also has a background as a developer and had his own company in the crypto field. 

Francesco Romeo is a FullStack Developer and has a university degree in Computer Engineering. He has several years of experience as a developer in different companies and accompanied as CTO and Founder the startup Buytime. The last years he worked as a FullStack Developer at the University of Applied Sciences in Bern. 

Simon Heer has worked several years in B2B Sales for RedHat and VmWare as well as in IT Risk and Compliance at AXA Insurance. He has a Master in Digital Business and Innovation and is responsible for the business aspects of the products. 


### Team Code Repos

- https://github.com/SayNode  A few repositories are private because of confidentiality agreements
- https://github.com/RsTs23
- https://github.com/wernerliechti
- https://github.com/Dohrnii-Foundation
- https://github.com/YannMarti
- https://github.com/paulamstutz


### Team LinkedIn Profiles

- https://www.linkedin.com/in/renato-sch%C3%A4r-8a9a19a5/
- https://www.linkedin.com/in/werner-liechti-568b19213/
- https://www.linkedin.com/in/paula-amstutz/
- https://www.linkedin.com/in/joaogmorais/
- https://www.linkedin.com/in/francesco-romeo-2867083b/
- https://www.linkedin.com/in/riccardo-mazzucchelli/
- https://www.linkedin.com/in/simon-heer-202866110/


## Development Roadmap 


### Example Roadmap for a dApp Application

#### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3 | Total |
| - | - | - | - | - |
| Estimated Duration | 45 d | 30 d | 30 d | 105 d |
| Full-time equivalent (FTE) | 2 | 1.5 | 1.5 | 5 |
| Cost (up to $ 30,000) | $ 15,000 | $ 7,500 | $ 7,500 | $ 30,000|


#### Milestone 1 — IPFS gateway

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | GNU Lesser General Public License v3.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial. |
| 1 | IPFS API and dedicated gateway | We will develop an IPFS API and dedicated gateway for users to be able to connect their applications to distributed storage. |
| 2 | Pinning service | The IPFS API will allow the files to be pinned and immutable even when the user is offline. |
| 3 | Compatibility | We will develop  IPFS API and dedicated gateway that are compatible with common tools, libraries, and frameworks, reducing the engineering. |
| 4 | Remove/Censor Content | Prevent certain types of content that are not suited for publication to be pinned to the IPFS service, such as child pornography. |
| 5 | Updatable URLs | We will give updatable URLs to the users which are human-readable. |
| 6 | Scalability | We will develop an IPFS infrastructure that allows scaling to users need. |

#### Milestone 2 - Performance and scalability upgrades

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | GNU Lesser General Public License v3.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial. |
| 1 | Snapshot system | A snapshot of the most current chain data will be taken. |
| 2 | Snapshot Storage | We will develop a Snapshot Storage that will store all the snapshots of the chain data and newly nodes can take the last snapshot to speed up the synchronization. |
| 3 | A validator | We will develop a validator that verifies if all the data is in the Snapshot Storage and if this data is corrupted or not. |


#### Milestone 3  —  Launch and operating and marketing costs

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | GNU Lesser General Public License v3.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial. |
| 1 | Launch | We will launch this service for the wider public. |
| 2 | Creating tiered subscription plans | We will create different tiered subscription plans to capture different needs. |
| 3 | Marketing campaign | We will create targeted ads and post on different platforms to capture the attention of developers from different ecosystems. |


#### Community engagement

For the community engagement, we will operate different channels simultaneously to achieve the widest possible reach. 

SayNode Channels: We will use our own channels to advertise. For this, a blog post will be made in collaboration with a freelancer for our website and blog. Then a post will also be made for LinkedIn. We will also regularly inform about the solution and its progress via Twitter. 

External Channels: In order to achieve the widest possible reach, we will use Medium. For this we will write an article at the respective milestones. We will also contact Truffle directly, as the solution promises advantages for them as well, we assume that they will be happy to use their channels to draw attention to the new possibilities. We will also make all posts directly available to VeChain, so that they can be used on your side if necessary. In addition, we will participate in events to draw attention to us. 

Website: We will create the products own website or expand an existing one. This will contain general information on pricing and functionality as well as a login and dashboard for users. It will allow users to use a free version or upgrade to one of the paid subscriptions. 

Paid Ads: In order for us to achieve a large reach, we will also make use of paid targeted advertising. For this we will use Google Ads. In order to achieve a certain impact, we assume a campaign over several months.

Monetanization: We will strive for a similar approach as Infura. Namely we will build in a pricing per project. So that there is no barrier to entry, we will provide a free version that allows to use the basic functionalities. If this version is no longer sufficient, a subscription to a "Pro-Version" can be purchased, which allows a larger number of requests. In order to have a solution for large projects or whole teams we will enable at least a third variant. For enterprise we will create an individual plan without an initial pricing that can be discussed directly. 

--> With the current data we assume that it will be built up as follows: 

|  | Free | $10/month | $20/month | Enterprise (individual pricing) |
| - | - | - | - | - |
| IPFS | 1 GB | 10 GB | 50 GB | individual |
| Projects | 1 | 10 | 15 | individual |
| Integration | -   | Truffle | Truffle | Truffle |
| URL | - | - | Upgradable | Upgradable |


## Future Plans

After the launch, the main focus will be to make the product known and to achieve the greatest possible impact. The goal is to win customers with different campaigns/outreach and create a solid user base. As soon as a certain number of users can be reached, the product will be further developed. Not only to meet the latest standards but also to integrate possible new developments or even to drive them forward ourselves. Always with the background to expand the ecosystem around VeChain. 

## Additional Information 

- What work has been done so far?

At this point, the first version V1 of our solution should be available. 

- Are there any teams who have already contributed (financially) to the project?

The project has not received any direct investment from other resources and is managed solely by SayNode Operations. 

- Have you applied for other grants so far?

This grant is a continuation of our solution and upgrade to V2. 
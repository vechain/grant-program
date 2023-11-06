# VeChain Grant Application - Dutch Carboneers App

## Project Overview 

- Project: Dutch Carboneers App 
- Team Name: SayNode Operations AG
- Payment Address: 0x989A38EDEbd2Bd80d4949a9F7462C93FA8055876

### Overview

- A brief description of the project

This project has been corporately planned by the companies Dutch Carboneers and SayNode Operations AG.

Dutch Carboneers develops decentralized biochar projects in the Global South in which local farming communities are provided with training, tools and technology to create biochar and carbon dioxide removal credits. All steps in the process are tracked with a mobile application and with that biochar production data, carbon credits are created which are sold on the voluntary carbon credit market. The process works as follows: Biomass is being collected and pyrolyzed into biochar by the farmers, after which the biochar is applied to the soil. Besides being a carbon sink for over a thousand years, biochar is a soil enhancer that improves water holding capacity, nutrient retention capacity and it increases the microbial activity in the soil, all leading to increased crop yield. On top of that, farmers are being paid for their climate services. Roughly 65% of the carbon credit revenue is rewarded back to the farmers. Thus far, 2 projects in India have been rolled out, working with over a thousand farmers, and to date 2500 tons of carbon dioxide have been sequestered for over a thousand years. To preserve high-quality Carbon Dioxide Removal (CDR), the traceability and transparency of our projects have to be really high. To track biochar production and the socio-economic benefits we have created our current mobile application with the help of our local implementation partner in India. It works, but it is far from ideal. All evidence of carbon sequestration and side benefits have to be tracked within one ecosystem, in the CDR world, this is often called digital Monitoring, Reporting and Verification, or dMRV for short.

SayNode is an established development company which offers blockchain-based mobile apps. The company is specialised in Web3, EVM-based blockchains and mobile wallets and it has completed several projects in this area. SayNode has applied for grants in the past, including for the development of the Thor Devkit for Flutter and for the development of the Mobile V3 Swap. In collaboration with Dutch Carboneers, SayNode wants to develop a solution which contributes to slow down climate change. SayNode is responsible for the technical implementation of the idea.

- An indication of why your team is interested in creating this project within the VeChain Ecosystem

It goes without saying that VeChain is a company with a great track record in enterprise blockchain solutions and as Dutch Carboneers’ projects are predominantly focussed on carbon sequestration, it is important that the footprint of the projects are low. It is therefore a major asset that VeChain's blockchain has a really low carbon footprint. On a personal level, I, Berend de Haas, have followed VeChain since 2017 and I know what the company is capable of and a lot of features that VeChain software offers to its clients fits right up the alley of Dutch Carboneers’ projects. Also the recently published whitepaper 3.0, web3 for better with its focus on sustainability and combining digital with physical aspects works well within the vision of Dutch Carboneers.

### Project Details

#### Definition of the Minimum Viable Product (MVP)

A blockchain-based app that helps farmers produce biochar, sequester solid carbon to slow down climate change and create Carbon Removal Credits in a more transparent, reliable and traceable way.
More transparency, credibility and traceability in the biochar production steps and more quality and trustful data collected, stored and shared in blockchain.

#### Tools and Features

The app will share and store information onchain in a credible and transparent way. The app needs to work offline because of the poor internet access in the locations. The main features will be:

- Basic personal information about the supervisor and the farmers
- Photos of each step of the biochar process made inside the app showing the geolocation, date and time stamp for more transparency and credibility
- Carbon data

#### Mockups/designs of any UI components

![Alt text](https://drive.google.com/uc?id=1nMmOfXipQPExZbtHq2sn34ZsNiqzJdqa) ![Alt text](https://drive.google.com/uc?id=1XYs7iSYmZbSNLPWpvWZ14uCCiuht8pL_)
![Alt text](https://drive.google.com/uc?id=1ApdrAFRPUsQV9N1qPvBeRgPxSoGe3Q_B) ![Alt text](https://drive.google.com/uc?id=1TGLNvle9Z_Brf7mSRi4cnaQ5jaTbw2mS)
![Alt text](https://drive.google.com/uc?id=12oB-UApI5qb25Cxdo0EqstEW1X27IOh_)

#### An overview of the technology stack to be used

The smart contracts will be fully written in Solidity.
The testing of the smart contracts will be done in Foundry in a locally run copy of Ethereum, and finally in real time with the VeChain testnet.
The backend will be written in Python, more specifically Django.
The frontend will be written in Flutter making use of the [thor-requests Dart library](https://pub.dev/packages/thor_devkit_dart), previously designed by our team.

#### Documentation of core components, protocols, architecture, etc. to be deployed

The project will have 1 main contract which will store all the required information for each user.

A Django application will help us to control the authorization and the accounts of each user, it will save the data while the user is offline and then send that data to Vechain as soon as a internet connection is established (this will be done using Django tasks and Celery).

The UI will allow the user (the supervisor) to easily take photos inside the app, see their account information and the farmers registered by them as well as the pictures of the biochar production steps, the biochar production overview, etc.

### Future Plans

Dutch Carboneers have two projects currently in operations. In November 2023, 4 more projects will be rolled out in different regions in India with the same local implementation partner with which the current projects have been set up. In the first half of 2024, we will travel to the African continent, setting up projects in Ghana, Malawi, Uganda and Kenya. These projects are drafted at the moment and the right implementation partners have been found already. In total, Dutch Carboneers aims to sequester 150.000 tons of carbon dioxide in 2024. The goal for 2028 is to sequester a million tons of carbon dioxide on a yearly basis. 

SayNode's future plans with the project are to create and distribute the app for smartphone devices, actively maintain the app, market it and build a loyal customer base. Future features that will be in discussion for implementation in the app are:
- Improve the profile page of the supervisors' and give them a better view of the farmers' profile
- Control the status of each biochar batch
- Integration of a handheld IoT moisture and heating temperature meter that communicates with the app
- AI picture recognition that can evaluate the pictures to control and automate the status of each biochar process and batch
- Mobile payment structure to pay supervisors and farmers directly via the app
- Dashboard with all data transparently presented for the buyers of carbon credits

The app is currently in the ideation phase where the first app mockups for a prototype was made. The team plans to develop a Minimum Viable Product (MVP) to validate the idea and gather initial user experiences. After the success of this project, SayNode is open to develop more software solutions based on the future plans of Dutch Carboneers.


## Team 

### Team Members

Dutch Carboneers contains a team of core people, interns and an advisory board, being the two co-founders the most revelant persons for the project:

- Berend de Haas, Co-founder and Biologist
- Mart de Bruijn, Co-founder and Environmental Economist

SayNode has about 25 employees. The most relevant persons (e.g. team leaders) for the implementation of the project are mentioned below. 

- Renato Schär, Co-founder and CEO
- Werner Liechti, Co-founder and COO
- Francesco Romeo, CTO
- João Morais, Senior Blockchain Developer
- Yann Marti, Senior Flutter Developer
- Paula Amstutz, Senior Blockchain Developer
- Rodrigo Dias, Flutter Developer

### Team Website

- https://www.dutchcarboneers.com/
- https://saynode.ch/

### Team's Experience

The co-founders Berend de Haas is a biologist and Mart de Bruijn is an environmental economist. A Chemical Engineer PhD will join Dutch Carboneers in Q1 2024, which will focus on the development of a more advanced, but still distributed pyrolysis machinery. Another PhD in Soil Science and International Agriculture will join Dutch Carboneers in Q2 2024, he will be in charge of the on-ground project development on the African continent. Furthermore, with the new mobile application for dMRV, we can engage in larger offtake agreements and hire a COO and CFO. For both positions, Dutch Carboneers has singled out the individuals and they are willing to join whenever called upon. Our local implementation partner must also be taken up in the team's experience, as he has over 25 years experience in working in the Odisha and Assam area on working with rural farming communities.

SayNode stands out for having the tech stack that combines blockchain and mobile development. We strongly believe that perfect user experience will be the key for a successful Web3 project. The team around SayNode has already implemented various projects in the Web3 area. A grant for the Dev-Thorkit-Dart as well as for the Mobile V3-Swap has already been granted and this project will include the same developers. Also, SayNode already deployed two Flutter Apps, which have been accepted in both Apple Store and Android Store. Overall, the team has experience with DAO creation, wallet creation, tokens and multichain tokens, ICOs and everything around App-Development.

### Team Code Repos

For confidentiality agreements no repo can be released for this project yet. As soon as the audit is complete, this will be made public. 

- https://github.com/SayNode/thor-devkit.dart
- https://github.com/SayNode/thor-request.dart
- https://github.com/SayNode/DAO-VeChain
- https://github.com/SayNode/axper
- https://github.com/SayNode/supply_chain_resilience_final
- https://github.com/SayNode/Vidaia
- https://github.com/SayNode/wizzer-flutter
- https://github.com/SayNode/FondueSwap
- https://github.com/JoaoMorais96
- https://github.com/Krfld
- https://github.com/RsTs23
- https://github.com/wernerliechti
- https://github.com/YannMarti
- https://github.com/paulamstutz

### Team LinkedIn Profiles

Dutch Carboneers:
- https://www.linkedin.com/in/berend-de-haas-25141b163/
- https://www.linkedin.com/in/mart-de-bruijn-770b90169/

SayNode:
- https://www.linkedin.com/in/renato-sch%C3%A4r-8a9a19a5/
- https://www.linkedin.com/in/werner-liechti-568b19213/
- https://ch.linkedin.com/in/francesco-romeo-2867083b
- https://www.linkedin.com/in/joaogmorais/
- https://www.linkedin.com/in/paula-amstutz/
- https://www.linkedin.com/in/krfld/
- https://www.linkedin.com/in/simon-heer-202866110/


## Development Roadmap

#### Overview

|                            | Milestone 1 | Milestone 2 | Milestone 3 | Total  |
| -------------------------- | ----------- | ----------- | ----------- | ------ |
| Estimated Duration         | 10 d        | 35 d        | 29 d        | 74 d   |
| Full-time equivalent (FTE) | 1           | 1           | 1           | 3      |
| Cost (up to $ 30,000)      | 5,000       | 15,000      | 10,000      | 30,000 |

#### Milestone 1 — Smart Contract development and test

| Number | Deliverable                                   | Specification                                                                                                                                                                                                                     |
| ------ | --------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0a.    | Documentation                                 | We will provide simple documentation for each contract, explaining their main functions and their roles.                                                                                                                          |
| 0b.    | Testing Guide                                 | The code will have proper unit-test coverage to ensure functionality and robustness. We will describe how to run both the Foundry and VeChain testnet tests.                                                                      |
| 1a.    | Smart Contracts: Development                  | We will develop the smart contract that will deal with data storage and management. We will open source the smart contract and upload the ABI to [B32](https://github.com/vechain/b32).                                           |
| 1b.    | Smart Contracts: Testing with Foundry         | We will create several tests in Foundry. Because Foundry allows us to run a mock up of the Ethereum blockchain and simulate the passage of time, we can run several tests in a matter of seconds, making it easier for debugging. |
| 1c.    | Smart Contracts: Testing with VeChain Testnet | We will preform all the previous tests in the Vechain testnet. This way we can make sure there is not functionality loss between blockchains.                                                                                     |

#### Milestone 2 — Backend

| Number | Deliverable               | Specification                                                          |
| ------ | ------------------------- | ---------------------------------------------------------------------- |
| 1      | Backend: Structure Design | We will design the app structure that will be implemented in Django.   |
| 2.a    | Backend: Development      | The previously planned design will be build and organized.             |
| 2b.    | Backend: Integration      | The backend will connect to the contract (and eventually the frontend) |
| 2c.    | Backend: Testing          | Several tests will be run to make sure everything works correctly      |

#### Milestone 3 — Frontend

| Number | Deliverable           | Specification                                                                                                                                                                         |
| ------ | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1      | Frontend: Design      | We will create the UI design of the MVP in order to make it appealing and intuitive. Colors schemes, button formatting, location of elements, etc, will all be done in this phase. |
| 2.a    | Frontend: Development | The previously planned UI will be build and organized.                                                                                                                             |
| 2b.    | Frontend: Integration | The frontend will connect to the backend.                                                                                                                                             |
| 2c.    | Frontend: Testing     | Several tests will be run to make sure everything works correctly: the UI works as intended and page load up speed/performance. The contract interaction is also checked.          |
| 2d.    | Frontend: Tutorial    | We will write a simple user guide for our MVP.                                                                                                                                        |

#### Community engagement

Dutch Carboneers has established quite a broad following on social media, specifically on LinkedIn, where we actively communicate about our projects, the Carbon Dioxide Removal and the biochar market as a whole. We also have a monthly mailing that goes to over 200 individuals in which the mobile application, Saynode and VeChain will be featured. Dutch Carboneers have been attending and presenting on multiple biochar and CDR related conferences and we have co-hosted one in the Netherlands in 2023. The product will bring great quality and value to our carbon sequestration projects and thus, it will be openly and actively shared who our partners are and how we can also help others with this mobile application. At the moment, we have 2 operational projects in India, but next year, the app will be also implemented in projects in Ghana, Uganda, Malawi, Kenya and Nigeria, and that is obviously not where we intend to stop. On a more local level, there is also a community effect created. We work with individual farmers, which are registered in the project. But these farmers are all part of larger farmer families. Every family can only participate with two family members in the project, but we have seen that they share the knowledge on biochar application. We hope that education and the word spreads on how their agricultural practices are improving their land. Not everybody will have direct contact with the project or product, but the community as a whole will profit from it. 

SayNode recently built a marketing team of 3 employees. The marketing team is in charge of creating content and organising webinars on social media platforms, mainly on Linkedin and X. In addition, we also play on different channels simultaneously and professionally, as well as using the platform Medium to write our blog. Thus, this project will be actively promoted on our channels by our marketing team. In addition, SayNode holds a Meetup once a month in Switzerland, where the products are promoted.


## Additional Information 

- What work has been done so far?
Dutch Carboneers is also already in contact with Tom Morris and Boyang Mao from VeChain to work on handheld IoT moisture meters for the supervisors in the project. This will be an important part of our dMRV model and will be integrated into the mobile application.

SayNode have already created the first mockups for the UI and have created also a roadmap and a rough project plan with the main features of our MVP.

- Are there any teams who have already contributed (financially) to the project?
No.

- Have you applied for other grants so far?
Yes, SayNode has requested VeChain grants in the past, but not for this project.

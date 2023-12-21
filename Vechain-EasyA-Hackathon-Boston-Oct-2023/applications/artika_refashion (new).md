# Vechain -Easy A Startup Grant Application Template
Hackathon Date: 7-8th Oct 2023

## Project Overview 
- Problem statement: BCG track
- Are you applying for the grant with the same project you submitted at the vechain Hackathon: Yes
- Project name: Artika Refashion
- Team name: Artika Refashion
- GitHub handle: Zibilicious
- College / Employer: Boston University
- Payment Address: 0x50545abB29D7e1724d04958eB2c31aBEF4227559

### Overview

We are Artika Refashion, a marketplace that connects independent fashion designers to users for fixing, upstyling, and innovating fashion. It all starts with a user's piece - a vintage jacket handed down from father to father, for example. This jacket has sentimental and monetary value but now needs upstyling or repair. That's where we come in: users can connect with fashion designers to customize or upgrade existing pieces, and the change is recorded on-chain, via NFTs representative of the clothing. Over time this will tell a story, which further adds value and expression to the piece.
With Artika 2.0, we directly partner with brands to create clothing tagged with NFTs. With this approach, we can include even more information about a piece, like verifying that its production is environmentally friendly or the materials used. At this stage, we can tie in loyalty tokens for exclusive content from brands, which further establishes them as environmentally friendly and rewards users for being a part of our platform. Vechain is a sustainable blockchain with EVM compatibility, low gas fees, and a focus on sustainability. With a rich ecosystem of libraries, would provide the best development and user experience.

### Project Details

- [BCG One-pager](https://docs.google.com/presentation/d/1Luw6KogeUF-JXmZVR5bVUMikw8UoAuFe/edit#slide=id.p1)
- [Pitch Deck](https://www.canva.com/design/DAFwn8CgBDg/FY_CvfOqyIX_y02IhlxmWg/edit?utm_content=DAFwn8CgBDg&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
- [UI Mockups/designs](https://www.figma.com/file/c6xrEmp5I8KnHepTvaHxwK/artika-refashion?type=design&node-id=0-1&mode=design&t=uaGC8cLWyiq9SIkn-0)
- [API specifications](https://github.com/IainWinter/Artika/blob/main/docs/api.md)

### Tech stack

- Smart contracts, written in Solidity, on VeChainThor.
- React Native frontend to create single codebase for all platforms (iOS, Android, Web).
- back4app BaaS to efficiently create, manage and scale backend resources.
- RESTful API backend made with back4app.
- Real-time database, provided by back4app, to store user data and link related objects.

### PoC
Our PoC was submitted to the VeChain/EasyA hackathon and can be found [here](https://github.com/IainWinter/ArtikaRefashion)

### Ecosystem Fit
We differ as the only fashion SaaS company in Web3, with a digital platform that connects independent fashion designers to users, promoting circular fashion by means of fixing, upstyling, and innovating fashion. Moreover, while sustainable supply chain tracking has been applied to many industries, no venture allows the consumer to view the product’s sustainable production and renovation history, to which they can contribute (sustainable supply chain tracking is introduced in Artika 2.0).

* Web2 Competitors:
  * Depop
  * Poshmark
  * Thredup
  * Stitch Fix
  * Fiverr
  * Upwork
  * Etsy

## Team 

### Team members

- Zi Zheng (Team Lead)
- Alika Grigorova (Project manager)
- Anna Sokolova (Project manager)

### Team Website

- [artikarefashion.com](https://www.artikarefashion.com/)

### Team's experience

* Zi
    * Zi has 4+ years of experience working cross-functionally developing and managing mobile apps and websites from marketing agencies and startups to global corporations like Goodyear and Bank of America.
    * https://www.zizheng.io/
* Anna
    * Anna has started multiple initiatives and held club leadership positions , as well as gained professional experience managing operations as an intern at Berkshire Hathaway HomeServices.
* Alika
    * Alika has worked as a project manager for non-profit initiatives, and gained professional experience as a financial analyst in a private business company.

### Team Code Repos

- https://github.com/IainWinter/ArtikaRefashion
- https://github.com/IainWinter/Artika

### Team LinkedIn Profiles

- https://www.linkedin.com/in/zi-zheng/
- https://www.linkedin.com/in/anna-sokolova-419a41273/
- https://www.linkedin.com/in/alika-grigorova-61159b281/

## Development Roadmap 

#### Overview

|                            | Milestone 1 | Milestone 2 | Milestone 3 | Milestone 4 | Total    |
| -------------------------- | ----------- | ----------- | ----------- | ----------- | -------- |
| Estimated Duration         | 30 d        | 60 d        | 30 d        | 20 d        | 140 d    |
| Full-time equivalent (FTE) | 2           | 2           | 1           | 1           | 5        |
| Cost (up to $ 30,000)      | $ 5,000     | $ 5,000     | $ 10,000    | $ 10,000    | $ 30,000 |

#### Milestone 1 — Backend & Smart Contracts
| Number | Deliverable       | Specification                                                                                                                          |
| ------ | ----------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| 1.     | Documentation | Create the full specification of our API and data requirements for the storage of text and images.                                          |
| 2.     | Smart Contracts   | Create smart contracts for adding tracking data points to an NFT. Provide an API for users to mint their own NFTs for their clothes |
| 3.     | Backend           | Create the backend API and a simple test suit.                                                                                         |
| 4.     | Simplest Frontend | Create a simple HTML frontend without any styling to gain an idea of our app's requirements for state management.                        |

#### Milestone 2  —  Backend
| Number | Deliverable      | Specification                                                                               |
| ------ | ---------------- | ------------------------------------------------------------------------------------------- |
| 1.     | Documentation    | Create in-depth documentation outlining API functionality (smart contract triggers, user authentication, data management). |
| 2.     | back4app         | Create resources (API, databases, test data, etc.) on the back4app platform, as outlined in the documentation.  |
| 3.     | Smart Contracts  | Create smart contracts for tracking user history stored on VeChain Thor (conducted on the VeChain testnet by interacting with a public node via the Thorest API). |
| 4.     | UI               | Create barebones UI in in react native to ensure basic frontend-backend communication. |
| 5.     | Unit Testing     | Conduct unit testing of all major functions and smart contracts to ensure business logic robustness. |

### Milestone 3 - Frontend
| Number | Deliverable        | Specification                                                                                             |
| ------ | ------------       | --------------------------------------------------------------------------------------------------------- |
| 1.     | Build UI           | Iteratively build frontend according to design mockups; Done on a per screen basis where functionality is consistent across all platforms. |
| 2.     | Connect Backend    | Install the ```Parse SDK``` via respective node module and initialize it using App Keys provided on the back4app website. |
| 3.     | Functional Testing | Ensure UI interactions propagate through API to trigger smart contracts and testnet updates. Similar testing for traditional database querying and updates. |

### Milestone 4 - Deployment & Marketing
| Number | Deliverable     | Specification                                                                    |
| ------ | --------------- | -------------------------------------------------------------------------------- |
| 1.     | Deployment       | Deplay app on the App and Google Play Store. Store compliance would have been verified in previous milestone while creating beta builds of the app.                                |
| 2.     | Write tutorials | Create blog posts on the website to teach new users how to best use our product. |
| 3.     | Marketing       | Create a marketing campaign to attract new users.                                |

## Future Plans

### Artika 1.0:
Build a decentralized platform to connect designers and users to facilitate sustainable fashion. Each piece of clothing will be represented as an NFT, each with a unique story, encouraging users to repair and upstyle their clothes instead of throwing them away.

### Artika 2.0:
Introduce a "sustainably produced" line of clothing, tracked through NFTs and historical records in the supply chain. Our tokenized loyalty system will include Early Access Tokens and VIP Event Access Tokens, which enhance demand and create unique opportunities for users. This collaboration is mutually beneficial, allowing luxury brands to build a "green" reputation without sacrificing profits while gaining new customers. ARTIKA 2.0 also enables users to trade redesigned clothing, boosting engagement and demand. Our long-term vision is to become the go-to social media app in the Web3 fashion industry for entertainment, inspiration, and services.

## Additional Information 

We have already created UI mockups and a pitch deck which was presented at the Vechain/EasyA hackathon at Harvard. We won 2nd place on the BCG track with these assets, and have edited them since then to reflect the budget and time available provided by this grant. We have not applied for any other grants. 

## Points of contact:
- Peter Zhou (Chief scientist at Vechain)
- Marina Fortunato (Project manager at Vechain)
- Bernhard Kronfellner (Boston Consulting Group)



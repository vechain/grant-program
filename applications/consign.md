# VeChain General Grant Application Template

## Project Overview 

- Project: Consign
- Team Name: Intharah 
- ETH Payment Address: 0x42B4935f07cD6e026FB96CA656Ae3Fdb09730191

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

ConSign v0.1.0:

Proof of Concept for the traceability of a product from the manufacturer/seller to the recycling company. Development of an incentive to recycle trash by rewarding all parties (consumer, selling and recycling companies) involved in a product lifecycle through blockchain technology.

Vechain has been chosen for the ease of implementation and the test environment available with Vechain Sync2. Programming language was also the main criteria as Vechain can be integrated directly into framework as Vuejs on contrary to other blockchains. The other point is obviously smart contracts which are relevant for the project.

### Project Details

The project repository can be found here (private repo - ask me first for granting access) :

https://github.com/intharah/consign

#### Expected final state and technical informations :

- Mockups/designs of any UI components

Coming soon

#### API specifications of the core functionality

Please see the document : <a href="https://github.com/intharah/grant-program/blob/master/applications/Consign%20API.pdf">API Specifications</a>

#### Documentation of core components, protocols, architecture, etc. to be deployed

- Environment :
node v10.24.1 || No upper version otherwise Vechain environment won't work
vue v2.6.14

- Front-end env :
bootstrap v5.1.0
bootstrap-vue v2.21.2
qrcode-vue v1.7.0
vue-router v3.5.2

- Back-end env : 
express v4.17.1
cors v2.8.5
mysql2 v2.3.0
body-parser v1.19.0

- Vechain environment :
Vechain Sync2
Connex 

<img src="https://github.com/intharah/grant-program/blob/master/applications/Consign%20-%20Infrastructure%20Diagram.jpeg" />

- PoC/MVP or other relevant prior work or research on the topic

Consign v0.1.0 has been inspired by the folowing article 'Blockchain Technology for Sustainable Waste Management' from Phillip Taylor, Katrien Steenmans and Ine Steenmans.

https://www.frontiersin.org/articles/10.3389/fpos.2020.590923/full

### Ecosystem Fit
Indeed, there are other competitors in this sector as 

    - Circulor : https://www.circulor.com/ , which makes a partnership with TotalEnergies Group (industrial-sized waste reduction)
    
    - Recereum : https://recereum.com/ , a blockchain-based platform for turning waste and recyclables to real value (no update since 2017)

But on contrary to them, I am focusing the waste reduction to the main target of the project, the final consumers by granting rewards if they bring their waste directly to the recycling company instead of throwing to the domestic trash bin.

## Team 

### Team members

- Name of team leader : Intharah
- Names of team members : Intharah (myself) but expecting collaborations in the coming months as this is my first project in the blockchain technology

### Team's experience

Intharah ACKHAVONG is a french UX/UI designer with over 15 years experience in IT. He has worked for digital departments of groups such as IBM or Sogeti in Luxembourg and recently for an innovative startup in France, Snaike, specialized in ML/AI for the medical sector. 

He participated in 2015 in a Hackathon Music in Metz as a designer for the project "Kraftwursht", prototype of a musical barbecue based on a moog synthetizer.

Intharah ACKHAVONG has taken part furthermore as an active member of a gaming association in the Northeastern of France and contributed in games creations during special game jam events. 

https://itch.io/jam/bbqgamejam15/rate/35801

One of his production, "Le chat de méliès", has been also registered in the BnF (Bibliothèque nationale de France), the French National Library as a digital creation.

https://data.bnf.fr/fr/17146365/le_chat_de_melies___jeu_video/


### Team Code Repos

- https://github.com/intharah/dodge-car-py // Arcade game, made in Python for a digital event in Metz "Vers l'infini et au-delà"
- https://github.com/VanschkliftEtLesThueringer/bbq // Musical barbecue with moog synthetizer, development in HTML5,JS,CSS3

### Team LinkedIn Profiles

- https://fr.linkedin.com/in/intharah-ackhavong-37998784

## Development Roadmap 

#### Overview

| | Milestone 1 | Milestone 2 | Milestone 3 | Total |
|-|-|-|-|-|
| Estimated Duration | 240 d | 120 d | 240 d | 600 d |
| Full-time equivalent (FTE) | 0.5 | 0.5 | 0.5 | 1.5 |
| Cost (up to $ 30,000) | $ 10,000 | $ 5,000 | $ 15,000 | $ 30,000 | 

#### Milestone 1 — Backend/Frontend developments x Smart contracts integration

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| Environment definition | Listing of frameworks, modules and libraries for the development environment |
| 0b. | Documentation | Inline documentation of the code |
| 1a. | Backend : Database structure | Complete schema of tables for each section (consumer/seller/recycling company) |
| 1b. | Backend : API | Creation of custom API for the backend services |
| 2a. | Frontend : Components | Development of front components for each section (consumer/seller/recycling company) |
| 2b. | Frontend : Assets | Stylesheets and visual elements |
| 3 | Connex | Implementation of Connex |
| 4 | Smart contracts | Local data registration into the blockchain via smart contracts |
| 5 | Dev version | Release of a development app |

#### Milestone 2  —  Economics

| Number | Deliverable | Specification |
|-|-|-|
| 6 | Peer review | Code analysis of the whole project |
| 7 | User design improvements | UX/UI feedback with external advisors |
| 8a. | Use case modeling | Specific scenarios for an inhouse company integration and feasibility Issues|
| 8b. | Business model | Development of an economic strategy |
| 9 | Partnership | Investigate for third-parties involvement |

#### Milestone 3  —  Proof-of-concept delivery

| Number | Deliverable | Specification |
|-|-|-|
| 10a. | Proof-of-concept | Release of a test version |
| 10b. | Test phase | Definition of the test (users group, duration, feedback tools) |
| 10c. | Validation phase | Fix relevant issues and build a stable deliverable |
| 11 | Infrastructure | Deployment for beta release |
| 12 | Marketing | Initiate a communication program |

#### Community engagement

As part of the Program, I will produce an article on Medium to explain and inform the work done after each milestone as part of the grant.

## Future Plans

If mid-term objectives are successful, I would manage to either hire qualified IT developer to build custom modules for the platform or find out a partner-associate with complementary skills.

Long-term plans intend on building a local ecosystem including industrial partners and governmental institutions for the promotion of waste reduction initiative. The Consign project will take part of the next step in the blockchain (r)evolution by including the technology in the real-life needs for the consumer and by innovating in sustainable solutions.

## Additional Information 

- What work has been done so far?

Vechain Sync 2 and Connex testing already done and Steps 0 and 1 are in the pipeline. Milestone 1 is in progress and project repository is built with initial structure.

- Are there any teams who have already contributed (financially) to the project?

Not at this time

- Have you applied for other grants so far?

Not at this time

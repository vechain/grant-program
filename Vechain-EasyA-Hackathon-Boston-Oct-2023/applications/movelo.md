# VeChain - Easy A Startup Grant Application Template

Hackathon Date: 7-8th Oct 2023

## Project

- Problem statement: Vechain track
- Are you applying for the grant with the same project you submitted at the vechain Hackathon: **Yes**
- Project name: Movelo
- Team name: Movelo
- GitHub handle: s-alad
- College / Employer: Boston University
- Payment Address: 0xD5bD5464Cb52dE2b3eeC76221f53d31f77825bC3 (Ethereum address, USDC prefered)

<!--
> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*
-->

## Overview

<!--
Please provide the following:
- A brief description of the project.
- An indication of why your team is interested in creating this project within the vechain Ecosystem.
- Link to project’s one-pager template (provided by BCG at the Hackathon).
- Link to pitch deck
-->

<div align=center>

<img src="https://media.discordapp.net/attachments/1158608110252982373/1165411327536287806/image.png?ex=6546c0e0&is=65344be0&hm=a43845184181d0d9cf8510a5ac93e78753deeb574a3b7ec91f5cb7dd2c10554b&=&width=1920&height=240" />

</div>

### Personal vehicles are among the prime contributors to global warming, largely due to their carbon dioxide emissions. Yet, there are no significant deterrents preventing individuals from overusing their cars. Many prefer the convenience of driving, even for short distances, over walking or biking. Enter Movelo.
  
**Movelo offers businesses a platform to craft campaigns that reward customers and employees for eco-friendly travel. Our vision is to spearhead a radical shift in transportation habits.**  
We harness the power of blockchain for instantaneous payments and the automation of transactions. On the other hand, server-side technologies validate the method of travel. Businesses can craft campaigns, either for the public or their workforce, which are then logged on the blockchain. Users, through our app, can view and participate in these campaigns by opting to walk or cycle to the respective destinations. The app monitors the journey, ensuring the travel remains sustainable, and upon completion, users receive payments in their chosen crypto wallets.

**Yet, there's a challenge: network growth. How do we entice businesses without a substantial user base, and vice-versa?**   
Our solution is a phased growth strategy. Initially, we'll target employees who are already commuting sustainably and businesses keen on bolstering their sustainability credentials. Gamified features, such as leaderboards and NFT badges for streaks, will boost user engagement and retention. As our community of daily commuters expands, we'll roll out our services to the broader public, luring more businesses onboard.

**In the long run, our ambition extends beyond the app.**    
We aim to influence a large segment of the population to adopt sustainable commuting habits, thereby prompting a shift in public infrastructure priorities. Imagine a world where roads and cities aren’t primarily designed for cars, but for sustainable modes of transportation. This could revive the positive feedback loop of sustainable transit, much like cars have dominated infrastructure planning for the past century.


[![](https://img.shields.io/badge/One_Pager-d?style=for-the-badge&label=&logoColor=ffffff&color=ffffff&labelColor=6A7EC2)](https://docs.google.com/presentation/d/1xXQmkTKioN5IuQTVCYqbnT55RFVIlmJ_wWzC9SVo7uE/edit?usp=sharing)  
[![](https://img.shields.io/badge/Pitch_Deck-d?style=for-the-badge&label=&logoColor=ffffff&color=099C09&labelColor=6A7EC2)](https://docs.google.com/presentation/d/1OeaLf-rTjphNoEQAoh7v_EMksedZmEpZ/edit?usp=sharing&ouid=108676669343177286257&rtpof=true&sd=true)

## Project Details

### MVP Screenshots & Design 

![](https://media.discordapp.net/attachments/1158608110252982373/1165446972761706527/image.png?ex=6546e213&is=65346d13&hm=d21e57434eb6211df196bbf440a30c7bb32a20f8291dd52c098209ce0dd8cfb1&=&width=1752&height=1002)

_*Design will be improved upon & is subject to change as we continue to develop the app & tackle milestones_

### Current MVP & Code
> **https://github.com/s-alad/movelo**  
> _Contains the mono-repo for the current MVP. MVP Frontend & Website & Backend + Contract are built out, but will be fully connected together, and improved as we start tackling milestones._

### Tech Stack

> **Client**  
> -React Native & Expo + Typescript  
> -NextJs + Typescript  
> 
> **Backend**  
> -Nodemailer Email Function  
> -Smart Contracts + Solidity  
> -Hardhat / Foundry  
> -GCloud Functions  
> -NextJS Edge Functions  
> -Express.JS Server  
>  
> **Storage**  
> Firestore  
> GCloud Bucket Storage  
>
> **Analytics**  
> Umami & Vercel Analytics  
>
> **Apis**  
> Google Maps Api  
> Native Location Phone API    
> Connex.js 
> Web3.js / ethers.js
>
> **Auth**  
> VeWorld Auth  
> Email + Passwordless  
> Google OAuth  


### Architecture
> ```
> ├── React Native & Expo App   
> │   ├── Native Mobile API Location Data  
> │   ├── Google Maps Api for directions
> │   ├── Ethers.js, Web3.js, Connex.js
> │   ├── Calls to Smart Contract
> ├── Server  
> │   ├── Firebase Cloud Functions
> │   │   ├── Fee Delegation Fxn
> │   │   ├── NFT Creation  
> │   │   ├── Ethers.js, Web3.js, Connex.js
> │   │   ├── Calls to Smart Contract
> │   ├── FireStore
> │   │   ├── Social & Friends Database
> │   │   ├── Email Correlations
> │   ├── OAuth
> ├── Smart Contracts  
> │   ├── HardHat / Foundry Compilation
> │   ├── ERC721 NFT (Coupon / Prize) Contract  
> │   ├── Movelo Sponsor & Payout Contract
> ├── NextJs Site
> │   ├── Sponsor Portal
> │   ├── Calls to Smart Contract
> │   ├── Edge Functions
> │   │   ├── Mailing List
> │   │   ├── Contact Forms  
> │   │   ├── Community & Blog  
> ```

### Current Documentation

_These are the current App & Contract functionalities. Many will be rehauled and more functions will be added to expand the app's capabilities._

#### Contract

> **Campaign**  
> a sponsorship campaign that contains information & monetary value

> **Badge**  
> an achievement badge for a user

> **TangibleReward** : todo  
> a tangible reward for a user

> **events**  
> event SponsorshipCreated  
> event Payout  
> event BadgeEarned  
> event EmergencyStopActivated : only owner
> event EmergencyStopDeactivated : only owner

> **/createSponsorship**  
> allows a spnonsor to create a new sponsorship 

> **payout**  
> pays a user for a trip based on the sponsorship

> **awardBadge**  
> awards a user an achievment badge  

> **/campaignRunning**  
> checks if a current sponsorship campaign is running  

> **/withdrawUnspentFunds**  
> allows a sponsor to withdraw unspent funds from their campaign  

> **/getAllCampaignLatsLongs**  
> returns all campaigns latitudes and longitudes  

> **/getNearby**  
> returns all nearby campaigns to a given location  

> **/getFeatured**  
> returns all featured campaigns  

> **/getMyCampaigns**  
> returns all campaigns a user is a part of  

#### App

> **logging in**  
> a user connects to the VeWorld wallet to provide their identity  
> a user further connects their email for alternative login methods  

> **add friends**  
> a user can add friends to their friends list

> **viewing campaigns**  
> a user can view all nearby campaigns, featured campaigns and campaigns they take part of  

> **joining campaigns**   
> a user can join a campaign and start earning rewards  

> **sucessful trip / failure**  
> a user can complete a trip and earn rewards or fail a trip and not earn rewards  

> **viewing rewards**  
> a user can view their rewards and badges

#### Server

> **/createNFT**  
> creates an NFT reward for a user

> **/delegateFee**  
> delegates the gas fee between the sponsor & user

<!--
We expect the teams to already have a solid idea about the project's expected final state.
Therefore, we ask the teams to submit (where relevant):
- Mockups/designs of any UI components
- API specifications of the core functionality
- An overview of the technology stack to be used
- Documentation of core components, protocols, architecture, etc. to be deployed
- PoC/MVP or other relevant prior work or research on the topic
-->

## Ecosystem Fit

<!--
Are there any other projects similar to yours? If so, how is your project different?
-->
One company that closely mirrors Movelo's business model is **Sweatcoin**, which incentivizes outdoor walking by awarding users tokens redeemable for rewards, typically free trials or coupons for various online products. However, Sweatcoin has faced challenges in scaling their platform, largely due to the network effect and public skepticism towards a product offering 'free' items, as delineated in our overview.

To sidestep these hurdles, our strategy, as elaborated in our overview and slide deck, zeroes in on the existing employee-to-employer market. By targeting this market, we aim to entice larger businesses that stand to gain substantially from heightened traffic and an enhanced reputation. Unlike Sweatcoin, our rewards will go beyond mere 5% discount coupons and free trials, which we believe will foster public trust.

In the long-term, we envisage competing with mapping apps like Google Maps, Apple Maps, albeit only in non-automotive and non-public transit domains. The unique proposition we offer is compensating users for utilizing our app, as opposed to the conventional model. This monetary incentive places us in a favorable competitive stance; competing apps would need to match or surpass our 'free money' offer to retain a comparable user base. Our platform's distinctive approach not only promises to disrupt the market but also positions us distinctly against potential competitors in the mapping app sphere.

## Why Vechain?
VeChain's groundbreaking dual-token system, known for its exceptionally low transaction costs, aligns seamlessly with our operational needs. Our integration of VIP191 not only simplifies user onboarding but also empowers newcomers to dive in without the constraints of initial wallet capital. Smart contracts offer both automation and scalability, poised to help our app scale as swiftly as we acquire customers. Our shared emphasis on sustainability is further highlighted by VeChain's unwavering commitment to eco-friendly practices. This synergy underscores our choice of VeChain as the foundational blockchain, reinforcing our company's ethos of sustainable innovation.

## Team

### Team members

CEO: Wes Jorgensen  
CPO: Collin Barber    
CTO: Saad N.  

### Team Website

**https://movelo.app**  
**https://github.com/s-alad/movelo**

### Team's experience  

**Wes Jorgensen**  
> Current student at Boston University studying Economics and Computer Science  
> Current VP of Innovation @ Boston University Blockchain

**Saad N.**  
> Previous intern @ Google  
> Previous Software Consultant @ Better.com  
> Current VP of Technology @ Boston University Blockchain  

**Collin Barber**  
> Previous Computer Science Tutor @ PennState   
> Current student at Boston University studying Computer Science  
> Freelance Software Development


### Team Code Repos

**Saad N. (s-alad)**  
>
> [TooFake (repo)](https://github.com/s-alad/toofake)  
> Created [TooFake](https://toofake.lol) a reverse engineered BeReal client. Reached over **2 million** users & **80 stars** on Github.
>
> [NYC Aerospace](https://nycaerospace.vercel.app/index.html)  
> Co-Founder, & Handled the technical & team aspects of NYC Aerospace, an Aerospace research lab & 501(c)(3) organization. Expanded to 7+ of the best highschools in NYC. 
> 
> [Voices Of Africa](https://www.liquidbarriersolutions.com/voa/voices-of-africa)  
> Currently working on a platform to share and amplify the various voices of Africa. Over 600 Monthly Active Users

**Collin Barber (CJCrafter)**
> 
> [WeaponMechanics](https://github.com/WeaponMechanics/MechanicsMain)  
> Server software used in over 20 countries
> **1000+** daily unique users
>
> [ChatGPT Java API](https://github.com/CJCrafter/ChatGPT-Java-API)  
> Over **40 stars** on github, used by mobile developers

**Wes Jorgensen (wjorgensen)**
>
> [Escrow Contract](https://github.com/wjorgensen/Escrow-Contract)  
> An improved version of the OpenZepplin Escrow contract with third party authentication
>
> [617DAO](https://github.com/wjorgensen/617DAO/tree/main)  
> The DAO used by Boston University Blockchain club for club governance

### Team LinkedIn Profiles

[![LinkedIn](https://img.shields.io/badge/Saad_N-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/saad70/)  
[![LinkedIn](https://img.shields.io/badge/Collin_Barber-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/collin-barber-14489524a/)  
[![LinkedIn](https://img.shields.io/badge/Wes_Jorgensen-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-weston-jorgensen-b5530a20b/)

## Development Roadmap

<!--
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
| - | - | - | - |
| Estimated Duration | 30 d | 30 d | 60 d |
| Full-time equivalent (FTE) | 2 | 1 | 3 |
| Cost (up to $ 30,000) | $ 5,000 | $ 10,000 | $ 15,000|

#### Milestone 1 — Smart Contract & Backend

| Number | Deliverable | Specification |
| - | - | - |
| 0a.| License | Apache 2.0 / MIT / Unlicense |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial that can interact with the deployed smart contracts and backend service. |
| 0c. | Testing Guide | The code will have proper unit-test coverage (e.g. 90%) to ensure functionality and robustness. In the guide, we will describe how to run these tests |
| 1 | Smart Contracts | We will develop smart contracts that will...  (Please list the functionality that will be coded for the contracts) . We will open source the smart contract and upload the ABI to [B32](https://github.com/vechain/b32). |
| 2 | Backend | "We will create a backend service that will... (Please list the functionality that will be coded for the backend)" |

#### Milestone 2  —  Frontend
| Number | Deliverable | Specification |
| - | - | - |
| 1 | User Guide | We will provide a user guide or a demo video to show what features have been done.  |
...
-->
|                    | Milestone 1 | Milestone 2 | Milestone 3 | Total |
|--------------------|-------------|-------------|-------------|-------|
| Estimated Duration | 60 days | 60 days | 30 days | 150 days |
| FTE                | 1.5 | 1.5 | 0.5 | - |
| Estimated Cost     | $10,000 | $12,000 | $8,000 | $30,000 |

#### Milestone 1 - Smart Contract/Backend

| Number | Deliverable       | Specification                                                                                                  |
|--------|-------------------|----------------------------------------------------------------------------------------------------------------|
| 0      | Documentation     | Refactor code to be self documenting. Code will be navigable, and covered by unit tests where applicable.      |
| 1      | Smart Contracts   | Deployed on test net with unit test coverage. Contracts will facilitate creation of campaigns and hold information about them, handle transactions, and distribute and hold information about users NFT's |
| 2      | Security          | Users in a campaign will be consistently tested to make sure they are not abusing the system. Built in limits. |
| 3      | User Verification | We will create a system to allow users to login with their company email and associate their wallet address with their email |
| 4      | Connection to VeWorld| We will connect users VeWorld wallets to Movelo for both authentication and to facilitate payments |
| 5      | Implement Fee Delegation| We will continue and build out a system to delegate gas fees to employers |

#### Milestone 2 - Frontend

| Number | Deliverable    | Specification                                                                                                     |
|--------|-------------------|----------------------------------------------------------------------------------------------------------------|
| 1      | User Interface | Improve user experience, improve flow between menus, easy swiping, multi-finger swipes, etc.                      |
| 2      | Graphic Design | Commission and design graphics for buttons, map widgets, and current location                                     |
| 3      | Improve maps   | Improve Map appearance, reduce clutter on maps, reduce google api usage, notify direction changes                 |
| 4      | Gamification   | Add per-company leaderboards to encourage competition                                                             |
| 5      | Badges         | Show NFT badges for milestones, daily streaks, and for loyalty (encourage users to sign in often)                 |
| 6      | Social         | Add an in app social feature. easily share to social media platforms for increased engagement and user traffic    |


#### Milestone 3 - 1.0 Release

| Number | Deliverable     | Specification                                                                                                    |
|--------|-------------------|----------------------------------------------------------------------------------------------------------------|
| 1      | Test Coverage   | Unit tests to ensure functionality                                                                               |
| 2      | Incorporation   | Incorporate company and setup company bank accounts                                                              |
| 3      | Launch          | Launch the app on the Apple App Store and Google Play Store                                                      |
| 4      | Marketing/Sales | Cold calling ESG managers, prepare pitches, levy connections to put the app in use                               |


### Community engagement
[![](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/MoveloApp)  
[![](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/channel/UCO2fHviwGpeJOq2tcLgptKw)

<!--
As part of the Program, we require that you produce and publish at least one article/tutorial (e.g., on Medium). It
should explain your work done as part of the grant.

Please provide a link to your Twitter, YouTube, website or Medium article.
-->

## Future Plans

### Expansion

**ESG**  
Use CO2 saved and usage statistics from current companies as a selling point to onramp more customers. If companies opt in publicise company CO2 data through a `FETCH` API and on our website. 

**Media**  
Increase Media presence through Twitter and YouTube releases.

### 2.0 Release 

**Public Release**  
Allow the public to use the app, and allow anyone to create a campaign. With an existing userbase
from employees, companies will be more likely to join and use our platform to advertise and publish public campaigns. We can then advertise those public campaigns to bring more users in. 

**API Integrations**  
We will also integrate the API's of bike shares like BlueBikes and CitiBike for move verification & an increased userbase possibility.


### 3.0 Release

**Mapping**  
Once we have significant daily traffic in the app we can continue to expand our userbase by starting to reexamine how we can make mapping better. We can integrate new features like in addition to using google's maps directions, we can integrate AR directions via the camera, create or purchase our own map instead of using googles, and use previous user data to improve directions. We plan to break down mapping to first principles and build the best mapping app for walking and biking possible. This will also allow us to break into the mapping market.


## Additional Information

<!-- 
Any additional information that you think is relevant to this application that hasn't already been included.

Possible additional information to include:

- What work has been done so far?
- Are there any teams who have already contributed (financially) to the project?
- Have you applied for other grants so far?
-->
### Movelo was started at the VeChain x EasyA hackathon at Harvard University and won first place.

We have already started on the front-end and backend at the hackathon but given our re-evaluation to move from the general public first to just employees/employers first we will need to do some restructuring. We will also have to fix login & authentication. There has already been some money spent by our team to buy domains, cloud computing, and revamp branding.

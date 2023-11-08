# VeChain General Grant Application Template

## Project Overview 

- Project: Cypress
- Team Name: Team Cypress
- Payment Address: USDC (ERC 20) payment address. We don't accept payments for the program in other currencies at this stage. 0x55D5B91fDbEc14D372b3a79fb1A13d8e26B169ed

### Overview

#### Description
Cypress is a dApp that we have developed with Vechain that utilizes cryptocurrency to incentivize users to make sustainable travel choices. Our project aims to be a part of the solution to the environmental degradation that is caused by urbanization and the increasing levels of carbon emissions in cities. Consumers may not produce the majority of pollution but they are the majority of the population– Cypress allows conscious consumers to be a part of a community that values sustainability on every level. On Cypress users can build their own virtual garden for simply traveling sustainably. Cypress uses 3rd party integrations from sustainable transportation companies such as Uber, MBTA, and BlueBike in order to verify that users have taken one of those forms of transportation. From there, Cypress uses Vechain technology to distribute VET to those users. This VET can then be used within the app to purchase flowers for a virtual garden. Users can expand their gardens, unlock new flowers, complete challenges, and compare their impact with friends. We use Vechain to distribute the incentive in cryptocurrency which is highly secure and promotes a system with low carbon emissions. 

#### Why Vechain?
We enjoy working with Vechain tokenomics and transaction speeds. Because our app is heavily based on user gamification and usage of $VET for rebates and transactions, Vechain’s two token system was a perfect fit. In this sense, we do not have to deploy and create liquidity for our own fungible tokens and instead tap into the rich ecosystem for $VET, the native token itself. On the other hand, since $VTHO gas token is cheap and composable, users can freely interact with our app, buy many items, and book many trips without worrying about incurring crazy additional costs. Finally, we tap into the sustainable partnership ecosystem that Vechain has created, and we will get more direct access to bigger public transportation companies for partnership and integration into our platform!

We also plan to integrate VeChain’s Designated Gas Payer to allow our partnered companies to sponsor their users’ gas fees. This would encourage more active users, and also help onboard new users because they wouldn’t have to own VTHO to use the Cypress App!

### BCG One pager
https://docs.google.com/presentation/d/1cttvY8K2jHcKmtGGC3P-XfJQaKQdPx_-/edit

### Pitch Deck
https://www.canva.com/design/DAFwoshzffw/z1hK9R1SEokgJ87e3lU17g/edit?utm_content=DAFwoshzffw&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

### Project Details


#### Initial UI
https://www.figma.com/file/llEhoaZHO4GR2qSks42yjW/Cypress?type=design&node-id=26%3A726&mode=design&t=n5m75MV4c1dACDjy-1
#### API specifications of the core functionality
##### User Management:
- POST /api/users/register: Register a new user account.
- POST /api/users/login: Authenticate and log in a user.
- POST /api/users/logout: Log out a user.
- GET /api/users/profile: Retrieve user profile information.
##### Garden Management:
- GET /api/garden/:userId: Retrieve a user's garden information.
- POST /api/garden/:userId/plant: Plant a new tree or add an element to the user's garden.
- POST /api/garden/:userId/harvest: Harvest rewards from the garden.
- GET /api/garden/leaderboard: Retrieve a leaderboard of the most sustainable gardens.
##### Transaction and Rebates:
- POST /api/transactions: Record a sustainable transportation transaction.
- GET /api/transactions/:userId: Retrieve a user's transaction history.
- GET /api/transactions/rebates/:userId: Retrieve rebate $VET tokens earned by a user.
###### Sponsorship and Gas Fees:
- POST /api/sponsorship/:userId: Allow partnered companies to sponsor a user's gas fees.
- GET /api/sponsorship/offers: Retrieve a list of sponsorship offers for users.
###### Friend and Social Interaction:
- POST /api/friends/add: Add a friend to a user's network.
- GET /api/friends/:userId: Retrieve a user's friends and their gardens.
- POST /api/garden/:userId/share: Share a user's garden with friends.
##### Notifications:
- GET /api/notifications/:userId: Retrieve notifications for a user.
##### General Information:
- GET /api/app/info: Retrieve general information about the Cypress app and its features.
- GET /api/app/version: Check the app version and updates.
- POST /api/admin/ban/:userId: Admin action to ban a user or take other moderation actions.
- POST /api/admin/maintenance: Put the app in maintenance mode for updates.

## An overview of the technology stack to be used
	- Frontend: React Native v.0.72.5
	- Backend: GoLang as Backend API Server, Solidity
	- Database: Postgres
	- API Calls: Chainlink
## Documentation of core components, protocols, architecture, etc. to be deployed
We built a Progressive Web App (PWA) optimized for mobile users with React, Next.js. This is the same framework that Friend.tech was built with! Because we used the web app design, we can utilize the VechainThor Wallet as our Web3 Provider on mobile and access a URL of our app (that looks like its a mobile app). We then wrote our smart contracts using Solidity on Remix, and deployed them to the Vechain Testnet using an app called https://inspector.vecha.in. Finally, we used the @vechain.energy/use-vechain SDK to index Vechain block information and access functions in our smart contract ABI. We’re planning on adding Chainlink oracles to query user data in real time and update relevant data in our smart contract.

View our code thus far here: 

	- Frontend: https://github.com/Cypress-Protocol/frontend 
	- Backend: https://github.com/Cypress-Protocol/backend 
	- Web3: https://github.com/Cypress-Protocol/contracts
### PoC/MVP or other relevant prior work or research on the topic

This project was initially built for the vechain x EasyA hackathon held at Harvard University, where it finished 4th for the VeChain Sustainability track. For the purpose of this application, the project scope has been updated and adjusted accordingly in order to reflect a clear unique selling point (USP), and product market fit (PMF). Additionally, the infrastructure plans for both backend and frontend have been significantly improved.



### Future Plans

### 1. Expanded Partnership Network
To increase the platform's value proposition we aim to forge partnerships with sustainable transportation companies. These include but are not limited to UberShare, BlueBikes, Citibikes, Byrd, and the MBTA. Expanding our partnership network will expand our target audience and encourage users to use Cypress.

### 2. Blockchain Authenticity
Leveraging blockchain to provide $VET token rebates on user transactions ensures authenticity and provides transparency for conscious consumers. This app will contribute to the future of Web3 technology.


#### Long-term project Plans

We have many technological improvements and planned features to unroll. We have detailed these plans in our milestones.

#### Business / Operation Plans

Market Analysis- Allocating resources to increase the authenticity/validity of our market research, including demographic and competitor analysis as well as an accurate and thorough SWOT analysis for our app. 

Marketing Strategies- Creation of a marketing plan, including plans for digital advertising and social media presence to secure users as well as partnerships. Additionally, instilling engagement/retention plans that give premium subscriptions or unique discount incentives. 

Operations and Security- Solidifying app infrastructure to ensure customer support is available and data privacy and security measures are taken. 

Sustainability- Sustainability reports and integrating transparency with the sustainability of the production of our app, the companies we partner with, and the environmental contributions the app would make. 

Finances- Monitor the breakdown of operation, marketing, development, and management costs and assess sales forecasts, cash flow analysis, and funding requirements. 

### Ecosystem Fit
https://www.forestapp.cc/ 



## Team Cypress


### Team Members

- Name of team leader: Sean Cho
- Names of team members: Zile Cao, Vince Tiu, Jefferson Ding, Courtney Kreitzer, Kyra Holmes

### Team Website

- https://github.com/ZILECAO/Cypress 

### Team's Experience

Sean Cho - Experience developing comprehensive full stack applications in Web2 and Web3. Have implemented frontends using react, and coded backend logic using Solidity. Some projects I’m proud of are: luckyape and CharityChain (currently ongoing development on the SUI chain). I have entered 3 web3 hackathons to date! 

Zile Cao - Crypto-native full-stack developer since 2021. Current engineer at Metaversal Ventures and Director of Engineering at Penn Blockchain. Was previously a technical PM for Weavechain and ambassador for Solana Foundation. Previous founder of EthDenver Hackathon finalist project (Inheritable)[https://app.buidlbox.io/projects/inheritable]. 

Vince Tiu -  Current Computer Science and Business student at UPenn (4.0 GPA). I have over 7 years of experience as a coder working on various projects addressing social and technological needs. Software Engineer at Moonhub, Co-Director at Penn Blockchain, and Previous Software Engineer at Infura via Consensys. 

Jefferson Ding - Experience working with full stack web2 and web3 development as well as mobile development. Implemented fully deployed web apps and mobile applications. Experience with Solidity and using JavaScript frameworks like Web3.js or Ethers.js to create web based DApps. All my projects can be found on my [GitHub](https://github.com/JeffersonDing?tab=repositories).

Kyra Holmes - Comprehensive marketing experience and social media management, strategically increasing brand visibility and online presence. Experience in creative visual, video, and written content creation and utilizing data-analytics to assess audience behaviors, as well as basic programming experience in Python and Java. 

Courtney Kreitzer - Extensive design experience in Figma and AdobeXD. Certified in Coursera’s Google UX Design Course and current UX Designer for JumboCode at Tufts University. Some basic front-end experience. My design portfolio can be viewed on my website (https://courtneykreitzer.com). 

### Team Code Repos
Zile Cao (https://github.com/ZILECAO)
<br> Vince Tiu (https://github.com/vincetiu8) 
<br>Sean Cho (https://github.com/seanwjcho)
<br> Jefferson Ding (https://github.com/JeffersonDing) 

### Team LinkedIn Profiles
<br>Zile Cao (https://www.linkedin.com/in/zilecao/) 
<br> Vince Tiu (https://www.linkedin.com/in/vincetiu8/) 
<br> Courtney Kreitzer (https://www.linkedin.com/in/courtneykreitzer/)
<br> Sean Cho (https://www.linkedin.com/in/seanwjcho/ )
<br> Jefferson Ding (https://www.linkedin.com/in/dingjefferson/)
<br> Kyra Holmes(https://www.linkedin.com/in/kyraholmes/)


## Development Roadmap 


#### Overview

|  | Milestone 1 | Milestone 2 |  Milestone 3 | Milestone 4 |Total |
| - | - |- | - | - | - |
| Estimated Duration | 45 d | 60 d | 45 d | 10d |135d |
| Full-time equivalent (FTE) | 4 | 5 | 4 | 3 | 16 |
| Cost (up to $ 30,000) | $ 10,000 | $ 12,000 | $ 6,000 | $ 2,000 | $ 30,000 |


> *⚠️ Please note that milestone 1 funds cannot exceed 40% of the total amount you are applying for.*


### Milestone 1 - Research & Development, Design, Backend, Outreach

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Research | - Research consumers’ sustainability habits and desired workflow. <br> -  Speak with users of public transportation to gauge needs. |
| 2 | Integration | - Create clear and concise requirements for blockchain integration, product tracking, transparent sustainability metrics, and technical implementation |
| 3 | Outreach | - Contact potential investors such as BlueBike and Byrd to see if a partnership is possible. |
| 4 | Designs | - Conduct a competitive analysis and refine the current UI/UX system based on market research and necessary requirements set out by consumers and brands. |
| 5 | Backend Development | - Implement the core backend functionality of the Cypress app to support blockchain integration, user management, transaction processing, and sustainability tracking. |
| 6 | Backend | - Set up the Go-based backend environment and version control system.
| 7 | Integration | - Create API endpoints for user registration and authentication. |
| 8 | Frontend | - Develop the garden management system, enabling users to plant, grow, and harvest rewards.|
| 9 | Testing | - Test transaction and rebate processing. <br> - Test VeChain blockchain for transaction recording and rebate token management.| 
| 10 | Improvements |  - Enable sponsored gas fee support using VeChain's Designated Gas Payer. <br> - Set up notification handling |
| 11 | Testing and Quality Assurance | - Conduct thorough unit and integration testing for all implemented backend functionalities, ensure secure and efficient interactions with the VeChain blockchain. <br> - Test admin and maintenance features. |



### Milestone 2 - Technical Implementation + Frontend 


| Number | Deliverable | Specification |
|-------|-------|-------------|
| 1 | Smart Contracts | - Develop and deploy smart contracts.<br> - Implement functions for tracking user balances, owned digital assets, and automated reward disbursement.<br> - Create functions for updating on-chain user data based on sustainability metrics.<br> - Integrate functionality to represent user assets as NFTs.<br> - Add an oracle for obtaining sustainability metrics from partners. |
| 2 | Smart Contract Integration | - Integrate the deployed smart contracts with the frontend.<br> - Ensure the frontend can accurately display user assets.<br> - Implement a customizable and dynamic user garden that interacts with the smart contracts.<br> - Enable the frontend to track plant growth based on on-chain data.<br> - Create a social leaderboard using on-chain data. |
| 3 | Designs | - Create a comprehensive working prototype for the user interface and experience using Figma.<br> - Ensure the design is user-friendly, visually appealing, and aligned with the app's features. |
| 4 | Backend | - Integrate the smart contracts into the backend system.<br> - Develop functionality for NFT minting and burning upon payment transactions.<br> - Use a web2 payment processor, such as Stripe, to manage financial transactions.<br> - Ensure the backend is notified of all relevant transactions involving smart contracts. |
| 5 | Frontend | - Develop an initial prototype for the react-native app.<br> - Implement specialized code integrations for Sync2 Wallet connection, and backend API call integration.<br> - Utilize React native in conjunction with native Swift libraries, such as Combine, for efficient frontend development. |
| 6 | Backend | - Create a robust REST API infrastructure with custom endpoints to cater to mobile users and web frontend for brands.<br> - Ensure that the backend can handle user data securely and interact with smart contracts effectively. |
| 7 | Frontend | - Develop a web frontend for brands to visualize transaction data.<br> - Ensure that the web frontend provides a user-friendly interface for brand partners.<br> - Integrate data from the backend and smart contracts for accurate visualization. |
| 8 | Report | - Collaborate with the VeChain team and revise the prototype based on their feedback.  Address any technical or design concerns and optimize the app for the VeChain ecosystem. |

### Milestone 3 - QA Testing and Refinement

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Smart contracts | - Create additional functions for managing newly onboarded partners.<br> - Update oracle to handle data from these partners. <br> - Create a secure NFT transfer mechanism to allow trades between users if they wish to transfer their Cypress assets. <br> - Include “adding friends'' functionality to create a working social leaderboard and boost engagement. <br> - Integrate smart contract with vechain.energy API.
| 2 | Testing | - Thoroughly test the smart contract, focusing on access control, functions that involve transfer of funds or assets, and update of persistent data. <br> - Fuzz frontend with unexpected user behaviors, fix any bugs / crashes. <br> - Ensure backend is secure with penetration testing.
| 3 | Auditing | - Get a security audit of the smart contract done by a third party. Extremely important as we are creating assets with real value and automatically providing rewards in VET. 
| 4 | Report | - Incorporate feedback from the vechain team and edit application.
| 5 | UI improvements | - Conduct user research and have users test UI/UX in focus groups.<br> - Reiterate and improve UI based on results.
| 6 | Marketing| - Create a marketing plan to output cypress to the community including creating social media accounts, online advertising, and writing blog/tutorials for app usage. |


### Milestone 4 - Final Testing and Deployment

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Testing | - Conduct final tests to assess UI/UX and structural features to catch last minute bugs and make adjustments accordingly. |
| 2 | Launch |- Launch as an iOS app on the Apple App store ensuring that the app is in compliance with App Store Guidelines and gain approval for publishing |
| 3 | Marketing | - Follow through with marketing on social media, utilizing social platforms to connect with potential users as well as potential partners, keeping engaged with advertising and consumers behaviors to increase effective marketing strategies |
| 4 | Documentation | - Review all documentation. <br> - Spend significant time creating documents that will help onboard new users and answer commonly asked questions. <br> - Create video demos that help users understand how to use the platform properly |


#### Community Engagement

We will be publishing guides/tutorials, demos, and short updates on various social platforms. Guides/tutorials would be great on Medium. Demos could go on any social media, and Youtube. Our short updates (text-form) would be perfect for twitter. 

We’ll also be continuously tracking our progress and writing documentation as we go so our platform is easy to use.


## Additional Information 

This project was initially built for the vechain x EasyA hackathon held at Harvard University, where it finished 4th for the VeChain Sustainability track. For the purpose of this application, the project scope has been updated and adjusted accordingly in order to reflect a clear unique selling point (USP), and product market fit (PMF). Additionally, the infrastructure plans for both backend and frontend have been significantly improved.




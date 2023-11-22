# VeChain General Grant Application Template

Hackathon Date: 7-8th Oct 2023

## Project Overview 

- Project: Flybloc
- Team Name: Flybloc 
- Payment Address: 0xd83d7e802a9abdF6F33d61978579d49ab1d0061F

Flybloc is venturing into a new frontier of brand engagement through the medium of gaming. The initiative is rooted in a two-fold approach: fostering a deeper connection with our audience and delivering a rewarding user experience. The digital platform will host a suite of games that are simple, approachable, and designed for quick, engaging interactions. The goal is a fun user experience without demanding a significant time commitment. Beyond just gaming, the platform will seamlessly intertwine the world of blockchain, enabling users to earn rewards that can be redeemed for brand-sponsored discounts, exclusive merchandise, and unique experiences.

## Project Details

### Web3 Strategy
VeChain, with its dual-token system, offers an optimized balance between transaction costs and speed, making it an attractive solution for applications that demand swift and economical operations. By utilizing VeChain's low-carbon platform, FlyBlock can demonstrate a commitment to eco-friendly practices in our system operations. Furthermore, its established track record in supply chain management and product traceability offers robust tools and frameworks, which can be leveraged for transparent reward tracking and verification in our gaming platform. 

VeChain's capability to handle a high volume of microtransactions seamlessly and expediently would ensure that our users experience instantaneous blockchain interactions, whether it's earning rewards or redeeming them for brand-sponsored offers. As the product scales, we intend to leverage MTT for concurrent transaction handling.

During our tokenomics provenance period, fee delegation will be explored to offset transaction costs as compared to a chargeback to our partners. While our initial MVP is primarily exploring custodial wallets, Sync2 is a strong candidate for self-custody as we explore the most frictionless experience.

Finally, VeChain's compatibility with standard programming languages facilitates easier integration with our existing tech stack. This is especially true given our preference for javascript-based middleware and services, and the use of Connex is already being researched and tested.

## Architecture
Leveraging Unity3D as our cornerstone, the design encapsulates a primary UI/UX app interfacing with a mobile web full-stack. This ensures a smooth transition and interaction with various game modules. Integration with the Supabase API forms the backbone of our real-time score tracking and user data analytics. The games, though diverse, share common attributes of being engaging and easy to grasp. On the blockchain front, the platform is crafted to reward users for their interactions, with tokens that can be converted into tangible, brand-centric benefits. To top it off, our approach is built on simplicity, ensuring users engage with the brand and its rewards without being entangled in the intricacies of blockchain mechanics.

Please include the team's long-term project plans, operation plans and intentions.

These are the deliverables we submitted for the Harvard 2024 VeChain Hackathon. 

- [Project’s one-pager](https://drive.google.com/file/d/1-XyiktDbbNv989igzI_MBvY1fkbqWTZf/view?usp=drive_link) (provided by BCG at the Hackathon)
- [Pitch deck on canva](https://www.canva.com/design/DAFwpuolMIE/7p25-BR8dz5krOzmGsBThw/edit)
- [Figma Board PoC Mockup](https://www.figma.com/file/upzjkNfHciqb3zFB3wHcS0/FlyBloc-UI%2FUX?type=design&node-id=0-1&mode=design)

Mockup of our PoC
Extrapolated from the Figma board above, the following images represent our platform view and the individual games we are developing. For the VeChain grant, we are focused on testing components of this PoC on blockchain to optimize rewards and redemptions. The learnings from this PoC will inform the MVP build-out in 2024. Please note that this VeChain grant is sufficient for 1 game for testing purposes. We are drawing upon other funding sources to build out the games below.


![Mobile Device UI/UX](https://i.imgur.com/OdNnZT0.png)

![Golf Game UI/UX Mockup](https://i.imgur.com/B1bvRnP.png)

![Word Scramble UI/UX Mockup](https://i.imgur.com/Q0BTKuQ.png)

API Specifications
Our API will be further described in both the Supabase admin as well as a Swagger interface for development (internal only). We do intend to extend our API ecosystem to allow third-party developers and brands to utilize the platform for independent game/brand engagement, with a governance process to review add-ons and additional games.

The following is a very high-level (and mostly exemplar) listing of the core PoC/MVP domains within the API.

User Domain:
Authentication (Auth):
- POST /auth/signup: Register a new user.
- POST /auth/login: Authenticate and retrieve a user token.
- POST /auth/logout: Log the user out and invalidate the token.
- POST /auth/password-reset: Trigger a password reset for the user.
Profile:
- GET /user/profile: Retrieve a user's profile information.
- PUT /user/profile: Update a user's profile information.
- DELETE /user/profile: Delete a user's profile.
Settings:
- GET /user/settings: Retrieve user's account and notification settings.
- PUT /user/settings: Update user's account and notification settings.

Game Data Domain
Scores:
- POST /game/scores: Submit a new game score for a user.
- GET /game/scores/{userId}: Retrieve all scores for a specific user.
Contextual Data:
- GET /game/data/words: Fetch word library for games.
- GET /game/data/context/{gameId}: Fetch any game-specific context like level data, challenges, etc.

Leaderboards Domain
- GET /leaderboards: Retrieve top scores across all games.
- GET /leaderboards/{gameId}: Retrieve top scores for a specific game.
- GET /leaderboards/user/{userId}: Retrieve leaderboard position of a specific user.

Metrics Domain
- User Engagement:
- GET /metrics/user-engagement: Metrics related to user activity, like daily active users, retention rate, etc.
Game Performance:
- GET /metrics/game-performance: Metrics regarding game popularity, average playtime, etc.
Rewards Distribution:
- GET /metrics/rewards: Data on how many rewards (tokens) have been distributed, redeemed, etc.

Rewards and Blockchain Domain:
Token Rewards
- POST /rewards/claim: User claims rewards.
- GET /rewards/{userId}: Retrieve user's accumulated rewards.
Smart Contracts:
- POST /blockchain/execute: Execute a smart contract action, like distributing rewards.
- GET /blockchain/transactions/{userId}: Fetch a user's blockchain transaction history.

Miscellaneous Domain:
Notifications
- GET /notifications/{userId}: Fetch notifications for a user.
- POST /notifications: Send a notification (e.g., for game updates, leaderboard changes).
Feedback & Support:
- POST /feedback: Submit feedback or report issues.
- GET /support/articles: Fetch support articles or FAQs.


Technology Stack
- Gaming Engine: Unity3D is at the heart of our gaming development, chosen for its robust capabilities and wide platform support. This will be employed for both the primary UI/UX and the individual game modules.
- Web Integration: WebView facilitates the seamless integration of mobile web full-stack content directly within our Unity application. This allows for dynamic content updates and real-time engagement metrics.
- Web Development: VueJS and NuxtJS or NextJS are the chosen frameworks for developing the responsive web components, ensuring compatibility across devices and delivering a cohesive user experience.
- Backend Database and API: Supabase serves as our go-to backend, offering real-time database functionalities and APIs. This allows for swift data operations, particularly for score tracking and user profile management.
- Blockchain Integration: A blockchain layer will be incorporated, designed to handle game rewards in the form of tokens. These tokens can then be redeemed by users for various brand-related perks. The entire blockchain process is geared to be frictionless, not necessitating users to have any prior blockchain knowledge.
Authentication: Single Sign-On (SSO) capabilities will be integrated, enabling users to quickly onboard and log in using familiar platforms like Google, Apple, and Facebook.
- QR Code Integration: A QR scanner will be embedded to allow users to quickly launch games or avail special offers by simply scanning QR codes, making the engagement process even more intuitive.
- Blockchain & Smart Contracts: A blockchain solution will be used for game rewards, and smart contract development will underpin the mechanics of rewards distribution, ensuring transparency and security.

Core Components and Architecture
Frontend:
- Frameworks to structure the web application such as VueJS, NuxtJS and/or NextJS
Backend:
- Web3 Integration: Connecting the backend to blockchain networks for rewards processing.
API Layer:
- RESTful API: Facilitate communication between frontend, backend, and databases. Can use Next or Nuxt JS routing capabilities.
Database:
- Supabase PostgresSQL: For storing user data, game states, scores, and more.
Authentication:
- OAuth2.0: For Single Sign-On (SSO) capabilities with Google, Apple, and Facebook.
- JWT (JSON Web Tokens): Securely transmitting information between users and the server.
Blockchain:
- Smart Contracts: Custom logic for handling game rewards, redemptions, and other blockchain-specific functionalities.
Cloud and Storage:
- GCP (Google Cloud Platform): Hosting the backend, databases, and asset storage.
- Google Key Manager: For secure storage of keys and critical environment variables.
- CDN (Content Delivery Network): Efficiently delivering game assets and content to users worldwide.
Security:
- HTTPS/SSL: Encrypting data in transit.
- Data-at-rest encryption: Ensuring stored user data is secure.
- CORS: Configuring server-side cross-origin requests for additional security.

By combining these core components, the gaming platform will achieve a scalable, performative, and engaging user experience across various devices, while also ensuring security and ease of maintenance.

### Long-term project Plans
Starting Q2 of 2024, we will begining our MVP build out which we estimate to cost between $400-500K for 6 months of build. During this build, we will engage our pilot partners for design feedback. Our target customers are niche apparel and food/beverage businesses. In 2024, we will rely on our own network to customers and their investors. We have a strong network to begin this work. With seed funding (at least $2M) in late 2024, we will hire marketing and sales team to expand our reach. Our priority in these first few years is to feature a diverse set of niche and at least one marquee brand.

For this MVP, we will build out in-app purchase feature and marketplace capabilities. This will put us on track to become the first one-stop-shop, gamified e-commerce platform for consumer brands. As a one-stop shop, we will deploy “interactives” (games) to attract users to our platform and enable them to make in-app purchases using rewards they redeem during gameplay. All happens within 1 platform.

Below is our plan for MVP in 2024.

#### Post-Prototype Product Roadmap (MVP) Release Criteria (for MVP 2024 build out):

Core Functionality Completion:
- All planned game modules are fully functional and integrated into the platform.
- Complete Supabase API integration for user data and game scores.

Full Authentication Integration:
- Full implementation and testing of SSO with Google, Apple, and Facebook.

Blockchain Functionality:
- Live blockchain transactions for token rewards, with smart contracts handling rewards distribution and redemption.
- Custodial wallet integration that allows for a frictionless experience, with users able to earn and redeem tokens without needing knowledge of underlying blockchain mechanisms.

Performance and Stress Testing:
- System can handle the expected load for six months post-launch, with scalability plans in place.
- Game load times optimized for immediate play.

Security Compliance:
- Comprehensive security audit completed with no critical issues.
- Compliance with relevant data protection and privacy laws.

User Experience (UX) and Design:
- Refined UI/UX based on user testing feedback, ensuring a seamless and engaging experience.
- Accessibility features implemented and tested.

Quality Assurance:
- All critical bugs identified in testing phases resolved.
- Performance benchmarks met with consistent system stability.

Documentation and Support:
- Full documentation for platform use, including FAQs for troubleshooting.
- Customer support channels established and operational.

Market Readiness:
- Go-to-market strategy in place, with marketing materials prepared.
- Partnerships with brands for rewards are established, with a clear pipeline for redemption.

Legal and Compliance:
- All legal clearances obtained, terms of service and privacy policies drafted and in place.
Compliance with the regulatory requirements of operating regions confirmed.

The MVP should be considered ready for launch once all these criteria are met, ensuring that the platform is viable for public use and capable of evolving based on real-world usage and feedback.

### Ecosystem Fit

Flybloc draws inspiration from the user engagement strategies employed by loyalty platforms such as FiveStars and Loyalty Lion, which have mastered the art of customer retention and rewards redemption. It mirrors these platforms' abilities to entice users with a plethora of rewards, creating a cycle of engagement and gratification that keeps users returning. However, Flybloc transcends the traditional loyalty system by embedding these mechanics within an interactive gaming environment, much like what users find on casual gaming platforms such as Friv and Poki.com.

These latter platforms are renowned for their vast and approachable gaming libraries, appealing to a broad audience with their simple yet engaging content. Flybloc adopts this model of immediate accessibility and ease of play but innovates further by integrating blockchain technology to modernize the rewards and redemption process. The result is a platform that not only offers quick gaming gratification but also ensures that every game played contributes to a larger reward ecosystem.

Users on Flybloc don’t just play; they engage in a brand-affiliated journey where each action has the potential to be rewarded through a blockchain-based token system. This not only adds an extra layer of excitement to the gaming experience but also provides real-world value through discounts, merchandise, and exclusive experiences, all redeemable through the tokens earned by simply enjoying the games.

Unlike Friv and Poki.com, where the end of the game is the end of the experience, Flybloc extends the engagement beyond the screen. And while FiveStars and Loyalty Lion have pioneered reward-based engagement, Flybloc leverages the immutable and transparent nature of blockchain to enhance trust and security in the user reward process.

This convergence of casual gaming with a sophisticated, blockchain-powered rewards system positions Flybloc as a unique presence in the market. It doesn't just aim to capitalize on the existing demand for easy-to-play games and reward systems but seeks to create a new niche where the line between playing and earning becomes delightfully blurred, giving users a sense of ownership and investment that's unmatched in current offerings. Flybloc is set to become a trailblazer, crafting an environment where loyalty and play coalesce into a singular, revolutionary user experience.

## Team 

### Yefei Jin, Cofounder
[LinkedIn Profile](https://www.linkedin.com/in/yefeijin/)

Ex-PM @Nearpod; Harvard Doctorate and MBA @Boston Univ.
Yefei brings 8+ years of product management and startup operating experience. He advises numerous startups on AI strategy and was the former Product Manager at Nearpod, an edtech student engagement company that successfully exited in 2021. Yefei holds his doctorate and masters from Harvard where he studied organizational leadership and data science. He also has his MBA from Boston University Questrom School of Business and B.A. from the Univ. of Minnesota Twin Cities.



### Alex White, Cofounder
[LinkedIn Profile](https://www.linkedin.com/in/alexwhite829/)

Ex-MLB athlete; investor and finance; MBA @UNC Chapel Hill
Alex is a former CFO turned Venture Capitalist. As founder of Yhat Invest, Alex provides finance and strategic development services to startups and early-stage ventures. Among others, he has worked closely with JustLend Ltd., a UK-based loan services platform, since 2021. Alex holds his MBA from UNC Kenan-Flager Business School where he studied corporate finance. Prior to business school, Alex was a professional MLB athlete for 10 years.



### Brandon Wolf, CTO
[LinkedIn Profile](https://www.linkedin.com/in/wolfbrandon/)

CTO at Napster, FIFA+Collect, Algorand; USMC Veteran 
Brandon Wolf brings over 25 years of experience in technology and digital transformations. A USMC Veteran, he has served in key executive roles as Chief Architect, CTO and CPTO most recently at Intapp, Algorand, Napster, and FIFA+Collect. Brandon is also a Board Advisor for various startups in the Web3 and AI domains. His depth and breadth of experience, servant-leadership style and lifelong passion for technology has made him a pivotal figure in driving innovation and success in the digital space.

### Jennifer Ma, Brand Strategist
[LinkedIn Profile](https://www.linkedin.com/in/jennifer-jin-ma/)

Ex-Brand Manager @L’Oréal & Nestle; Masters @Harvard
Jennifer is a seasoned marketing professional and award-winning entrepreneur. She brings brand management experience from L’Oréal and Nestle. Most recently, she was the Founder/CEO of ‘Little Oasis’ (early childhood education), which she successfully exited in 2023. Jennifer holds her MEd. at Harvard and has a Conjoint BCom/LLB from the Univ. of Auckland. Jennifer has been recognized by the University of Auckland in 40 Under 40 and KEA’s World Class New Zealander.

### Douglas Solomon, Business Development
[LinkedIn Profile](https://www.linkedin.com/in/douglas-r-solomon/)

20+ yrs of B2B content marketing sales; 2 exits as founder 
Douglas has led three successful start-up ventures in Media and Education. As a publisher and partner with Parents Plus, Inc., Douglas developed Boston Parents and other parenting media properties. Upon the sale of Parents Plus, Douglas launched Solomon Media LLC, a Fintech firm for the Education sector. The firm’s assets were acquired by Nelnet Inc. and soon after Douglas launched EEV Education, a BD consultancy. Douglas is a graduate of Stonehill College and resides with his family in Durham NC.

### Sanjay Baskaran, Advisor
[LinkedIn Profile](https://www.linkedin.com/in/baskaran/)

Tech VC, PE op partner, ex Amazon GM, fintech CEO, board advisor ML/AI, mentor Harvard Innovation Lab, passionate about AR/VR & collecting in web 3
Sanjay Baskaran currently serves as an advisor to PE firms in fintech & data services. He is among the top users in the VeVe digital collectibles community and owns 4K+ digital collectibles. He has 20+ years’ experience scaling, growing & digitally transforming companies using cloud, AI, ML and other digital tools. His prior FinTech leadership roles include CEO of One Technologies, President of TaxAct, and General Manager of Amazon Cards. Early in his career he served as Visa’s head of analytics for North America and spent a decade at HSBC in various product, marketing & risk management roles. He is an avid technology investor and sits on the advisory board of The Broad College of Business Michigan State University.

### Arina Shulga, Legal
[LinkedIn Profile](https://www.linkedin.com/in/arinashulga/)

Partner @Nelson Mullins; practice in web3 & gaming; J.D. in Law @UPenn
As partner at Nelson Mullins, Arina brings advice and counsel for fintech startups that operate in the blockchain space (including NFT platforms, DAOs, gaming companies, and others). For her crypto clients, she advises on the regulatory aspects of operations, issuance of digital tokens, NFTs, creation of platforms, and other aspects of operations in the Web3 space. She also advises angel investors and venture capital funds when making investments into startups. Arina holds her J.D. in law from the Univ. of Pennsylvania.

### Team Website

- https://www.flybloc.com

### Team Code Repos

- [GitHub - Mobile App (private)](https://github.com/FlyblocDev/flybloc-mobile)
- [GitHub - Web Stack (private)](https://github.com/FlyblocDev/flybloc-web)
- [GitHub - Backend (private)](https://github.com/FlyblocDev/flybloc-supabase)
- [GitHub - Web-Based Game (private)](https://github.com/FlyblocDev/Slingshot)
- [GitHub - Unity-Based Game #1 (private)](https://github.com/FlyblocDev/ScratchGolf)
- [GitHub - Unity-Based Game #2 (private)](https://github.com/FlyblocDev/FlyScramble)

Our repositories are private while we are in stealth/startup mode. All smart contracts/chain interop coding will be open at MVP. We are happy to provide reviewer access to these repos during the evaluation period.

## Development Roadmap 

### Overview
These costs are estimates based on the development partner we have vetted and chosen. We are engaging with a firm that can deliver us post-PoC through MVP. We have already defined the scope and costs in detail including the headcount of various roles. Below is a summary of those costs and staffing. 

|   |  Milestone 1 | Milestone 2 | Milestone 3 | Milestone 4 | Total |
| - | - | - | - | - | - |
| Milestone high-level objective | Smart contracts, reward models, and backend | UIUX and frontend development | Game development | Testing and deployment | - |
| Full-time equivalent (FTE) | 1x smart contract developer 1x backend developer 0.5x product owner | 1x frontend developer, 0.5x uiux | 1x game developer | 1x QA 1x DevOps 0.2 BE developer 0.2 FE developer | - |
| Est. duration | 30 d | 30 d | 14 d | 20 d | 94 d
| Cost | $ 12,500 | $ 10,000 | $ 5,000 | $ 2,500 | $30,000

#### Milestone 1 - Smart contracts, reward models, and backend
##### All smart contracts, reward models and backend API are defined. During this process, we hope to get counsel from VeChain developer community if needed.

| Number | Deliverable | Description |
|-|-|-|
| 1 | SC | Smart contract for custody (account abstraction) wallet is completed. |
| 2 | Tokens | Smart contract for rewards (token) distribution is completed. It has burn functionality for used tokens. |
| 3 | SC | Tests for contracts are written. |
| 4 | SC | Smart contracts are deployed to the test network and are tested. |
| 5 | SC | Smart contracts API and integration for the backend are completed. |
| 6 | Backend | Backend APIs are completed: User application, Login, Registration, Lost password, User profile, On user registration, wallet is assigned to the user automatically, Leaderboards, Reward redemption (exchanging tokens for rewards) |


#### Milestone 2  —  UXUI & Frontend
##### UXUI and frontend integration are  completed.

| Number | Deliverable | Description |
|-|-|-|
| 1 | Frontend | UXUI and frontend integration is completed. |
| 2 | Design | All screens and designs are completed in Figma. |
| 3 | Design | All screens and designs are implemented in the frontend application. |
| 4 | Integration | Frontend application is connected to smart contracts and backend API. |

#### Milestone 3  —  Game development
##### 1 simple game is completed and integrated into the application.

| Number | Deliverable | Description |
|-|-|-|
| 1 | Game | Complete development of 3 Unity game. |
| 2 | API | Game is connected and integrated with smart contracts and backends. |
| 3 | Game mechanics | User can access to game after login, and rewards are distributed based on the rewards rules. |

#### Milestone 4  —  Testing and deployment
##### Application is tested and deployed to production.

| Number | Deliverable | Description |
|-|-|-|
| 1 | QA report | All MVP scenarios are tested. |
| 2 | Deployment | All production environments and CICD are completed. |
| 3 | Deployment | Application is deployed to the production servers. |
| 4 | Deployment | Any user can access and use the application. |

#### Community Engagement

We will publish our work here and on our website in the blog section
- https://twitter.com/flybloc
- https://www.flybloc.com/ 

Once our Proof-of-Concept phase begins, we will engage on Telegram for notifications, and Discord for community and social interactions.


## Additional Information 

We want to share that our intention for this grant is to test and deploy on VeChain to assess the feasibility of this blockchain for MVP. Without this grant, we will continue to build our PoC in a Web2 tech stack. If we are awarded this grant, our goal is to test the blockchain infrastructure and APIs and determine if we will leverage those tooling for our PoC that will feature additional games along with our platform UI that will contain all games. The budget for this VeChain grant is sufficient for 1 simple game (in Unity) although we are drawing additional funding for 3 additional games (2 in Unity and 1 in WebGL). Upon achieving our milestones successfully, we can apply the APIs developed to these additional games.

We have secured 3 pilot partners so far to test our prototype in early 2024. We expect to have a 4th by early next year. We have built one game using Phaser.js for demo purposes. We have one high-fidelity wireframe of a golf game for a golf apparel company (game currently in development in Unity). All game mechanics and scoring models have been defined and their build has started. We can share ERD diagram and game mechanics upon request.

We are currently bootstrapped with 1 grant from a local web3 accelerator. This VeChain grant will allow us to test our PoC on blockchain which we originally slated to do for MVP in 2024 pending the success of a PoC on a web2 tech stack. This accelerates our timeline with learnings on how to build on blockchain and reuse our codebase should we move forward with VeChain.

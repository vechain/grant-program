

  
# Milestone Delivery :mailbox:

> Only the GitHub account, which is responsible for the pull request of the accepted application is allowed to submit milestones. Don't remove any of the mandatory parts presented in bold letters or as headlines!

**The Ethereum address has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](../#milestone-delivery-process).**  

* **PR Link:** [#207](https://github.com/vechain/grant-program/pull/207)

* **Milestone Number:** Milestone 1

Please provide a list of all deliverables of the milestone extracted from the initial application and a link to the deliverable itself. Ideally all links inside the below table should include a commit hash, which should be used for testing.

| Number | Deliverable | Link | Notes |
| ------------- | ------------- | ------------- |------------- |
| 1. | Research |[Research Presentation](https://www.canva.com/design/DAF6cfFuufM/vcdMTYG8sdO6qLO6cJ7nWA/edit)| All consumer data and research available here, includes survey respondent data + desired workflow. Slides 1-7| 
| 2.  | Requirements |[Requirements Document](https://docs.google.com/document/d/1iFZB31XT41khzqHYUzkxCHCL0ov-M5TMTjD0i8L0lE0/edit?usp=sharing)| Clear and concise requirements for blockchain integration, product tracking, transparent sustainability metrics, and technical implementation|
| 3.  | Outreach |[Research Presentation](https://www.canva.com/design/DAF6cfFuufM/vcdMTYG8sdO6qLO6cJ7nWA/edit)| Contacted potential investors/partners such as Uber, BLUEBIKES, MBTA to see if a partnership is possible. Slides 11-14|
| 4.  | Designs |[Competitive Analysis](https://www.figma.com/file/xYG6HZh7j5H0acJYD8oKcr/Cypress-Competitive-Analysis?type=whiteboard&node-id=0-1&t=PGb3V4NISAxEFM49-0) + [UI/UX Details here](https://www.figma.com/file/llEhoaZHO4GR2qSks42yjW/Cypress?type=design&node-id=26:726&mode=design&t=Uev1HLic5YHzOJli-1) | Competitive analysis performed and refined the current UI/UX system based on market research and necessary requirements set out by consumers and brands.| 
| 5.  | Backend Development |[Images located here](https://docs.google.com/document/d/1G2ePQPoRpvChe3VCsnSWnrCHJGOV9wLnr72aPklMcrU/edit) + [Github Repo for frontend located here, contains backend Web3Auth integration](https://github.com/cypress-labs/leegal). Specifically within this repo, the core backend functionality is implemented [here](https://github.com/cypress-labs/leegal/blob/main/cypress/App.tsx), detailed writeup located [here](https://drive.google.com/file/d/1XNigfQsA9vIM39A7CqR_-pjjGJdnAGAP/view?usp=sharing)| Implement the core backend functionality of the Cypress app to support blockchain integration, user management, transaction processing, and sustainability tracking. | 
| 6.  | Backend |[Go-based backend here](https://github.com/cypress-labs/backend/tree/main)| Set up the Go-based backend environment and version control system.| 
| 7.  | Integration |[Demo Here](https://drive.google.com/file/d/17fu7obses7gZM2kR1pGqfb1ovSWXJpaY/view) |  This demo shows API endpoints are set up and tested. Integrates backend + smart contract + React Native frontend | 
| 8.  | Frontend |[Demo Here](https://drive.google.com/file/d/17fu7obses7gZM2kR1pGqfb1ovSWXJpaY/view) + [Repo containing React Native frontend code here](https://github.com/cypress-labs/leegal/tree/main/cypress) + [Figma file containing prototype and added UX/UI pages here](https://www.figma.com/file/llEhoaZHO4GR2qSks42yjW/Cypress?type=design&node-id=26:726&mode=design&t=Np7KkiHSMdNx9ojP-1)| Frontend contains skeleton code for developing the garden management system. Figma contains hi-fidelity versions of what the garden management system will look like and improvements to the social system. We've prototyped out what the garden management system will look like in our Figma (can click prototype to go through entire user workflow), and also worked out what this management system would look like once implemented. This is also functionality we've enabled on our smart contract. The brunt of our frontend development will occur next milestone.| 
| 9.  | Testing |[Updated smart contract supporting gas sponsorship located here](https://github.com/cypress-labs/leegal/blob/main/Contracts/Cypress.sol) + [documentation showing smart contract testing here](https://docs.google.com/document/d/10PIPJRmZqC33H8okxsj35sEwKSOcvxFmW7yBltfW_xw/edit?usp=sharing)| Tested smart contract functionality as shown in demo, in proper sequence to guarantee no  execution errors| 
| 10.  | Improvements |[Screenshots showing improvements here](https://docs.google.com/document/d/1cVSxOP0wQgoWftz-qZZZXN1tQO4z418hxLhh0g2Y7nw/edit?usp=sharing) + [deployed token contract here](https://explore-testnet.vechain.org/accounts/0x419d1de229bae98cfbb1439e3209c8164ca9b2b3/)| Enabled sponsored gas fee support using VeChain's Designated Gas Payer using Vechain.energy + funded testnet wallet for sponsorship. Also deployed smart contract that creates our own native token: $FERT| 
| 11.  | Testing and Quality Assurance |[Demo Video](https://drive.google.com/file/d/17fu7obses7gZM2kR1pGqfb1ovSWXJpaY/view)| Conducted thorough integration testing for implemented backend functionalities. Ensured proper integration through Web3auth React Native SDK + Connex + Thor dev kit.|
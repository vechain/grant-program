# Milestone Delivery :mailbox:

> Only the GitHub account, which is responsible for the pull request of the accepted application is allowed to submit milestones. Don't remove any of the mandatory parts presented in bold letters or as headlines!

**The Ethereum address has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](../#milestone-delivery-process).**  

* **PR Link:** https://github.com/vechain/grant-program/pull/195
* **Milestone Number:** 2

Please provide a list of all deliverables of the milestone extracted from the initial application and a link to the deliverable itself. Ideally all links inside the below table should include a commit hash, which should be used for testing.

| Number | Deliverable | Link | Notes |
| ------------- | ------------- | ------------- |------------- |
| 1 | Smart contracts | [Tracking Contract](https://github.com/jjjutla/FibreTag/blob/main/backend/contracts/contracts/Tracking.sol)| Develop the tracking smart contract, include functions for comprehensive product lifecycle management, implement stringent access controls to ensure only authorized users can perform actions, and construct a secure transfer mechanism to automate NFT ownership transfers upon product sales |
| 2 | Smart contracts | [NFT Contract](https://github.com/jjjutla/FibreTag/blob/main/backend/contracts/contracts/NFT.sol) | Develop digital twin NFT contract for the item and bridge with vechain.energy API |
| 3 | Backend |[Payment Integration](https://github.com/jjjutla/FibreTag/blob/main/backend/src/payments/List/index.tsx) | Integrate the contract into a backend to handle the NFT minting/burning upon payment and use a payment processor like Stripe to manage finances and notify the backend of transactions |
| 4 | Frontend | [Code directory of iOS Swift project](https://github.com/jjjutla/FibreTag/tree/main/ios) and [YouTube video](https://youtu.be/KkgJxR6IqD8) with short demo| Develop initial prototype for the iOS app. Creating specialized code integrations for Google OAuth, efficient NFC read/write, and backend networking integration using native Swift library Combine |
| 5 | Backend | [Endpoints](https://github.com/jjjutla/FibreTag/blob/main/backend/src/App/appendEnpoints/index.tsx) | Create REST API infrastructure with custom endpoints for users on mobile devices and brands utilizing a web frontend |
| 6 | Frontend | [Dashboard](https://github.com/jjjutla/FibreTag/blob/main/backend/src/App/LoggedIn/Admin.tsx)  | Develop web frontend for brands to use in order to visaulise transaction data |
| 7 | Report | [Report](https://docs.google.com/document/d/1V4ucJSSbfCUH3a5LGkjh1XApgK8KNwRhua8oZjBMEnA/edit?usp=sharing) | Revise prototype based on feedback from vechain team |
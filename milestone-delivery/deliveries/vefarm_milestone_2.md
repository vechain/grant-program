# Milestone Delivery :mailbox:

> Only the GitHub account, which is responsible for the pull request of the accepted application is allowed to submit milestones. Don't remove any of the mandatory parts presented in bold letters or as headlines!

**The Ethereum address has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](../).**

* **PR Link:** [VeChain grant proposal - VeFarm #161](https://github.com/vechain/grant-program/pull/161)
* **Milestone Number:** 2

Please provide a list of all deliverables of the milestone extracted from the initial application and a link to the deliverable itself. Ideally all links inside the below table should include a commit hash, which should be used for testing.

**Notice:** The app has been rebranded from VeFarm to vearn.

**Overview:** The project has been split into several repositories:

1. [client](https://github.com/vearnfi/client): Frontend for the vearn protocol. It is responsible for interacting with the Energy and Trader contracts and making calls to the backend.
2. [events fetcher](https://github.com/vearnfi/events-fetcher): Node service that listens to events associated with the vearn protocol and forwards them to the backend.
3. [backend/firebase](https://github.com/vearnfi/firebase): Serverless backend responsible for storing all data related to the vearn protocol, computing optimized strategies based on user balances and market conditions, and executing the swap method on the Trader forecast.
4. [config](https://github.com/vearnfi/config): NPM package containing all configuration values associated with the vearn protocol.
5. [contracts](https://github.com/vearnfi/contracts): Smart contracts associated with the vearn protocol.
6. [gas](https://github.com/vearnfi/gas): NPM package containing gas-related utility functions forked from vechain.energy.
7. [wrapped connex](https://github.com/vearnfi/wrapped-connex): NPM package with commonly used utilities built on top of connex.
8. [mathematical analysis](https://github.com/vearnfi/mathematical_analysis): Short article describing the mathematics behind the vearn protocol.

| Number | Deliverable | Specification | Link |
|-|-|-|-|
| 0a. | Documentation | Provide comprehensive inline documentation of the code and create a basic tutorial that demonstrates interaction with the deployed smart contract. | [https://github.com/vearnfi/contracts/blob/main/README.md](https://github.com/vearnfi/contracts/blob/main/README.md)
| 0b. | Testing Guide | Ensure proper unit test coverage (e.g., 90%) for the code functionality and robustness. Document the steps to run these tests in a testing guide. | Please, refer to the testing section inside each repository.
| 1 | Smart Contract | Build upon the Milestone 1 specifications. Restrict the access to the `swap` function to the contract's owner and likely some admin accounts (TBD). Integrate a list of accessible DEXs for trading, with immutable addresses set during contract initialization. Introduce a `dexId` parameter to the `swap` function, enabling the selection of a specific DEX for the swap. Upon function call, we deduct transaction fees and the protocol fee (0.3%), and then swap the remaining amount for VET, sending it directly to the user's account. Enable the contract owner to withdraw accumulated fees. | [https://github.com/vearnfi/contracts/blob/main/contracts/Trader.sol](https://github.com/vearnfi/contracts/blob/main/contracts/Trader.sol)
| 2 | Backend | Build upon the Milestone 1 specifications. Develop an algorithm to optimize the swap timing based on market conditions and account balance. It should outperform a fix time interval swap strategy. ~~Compute the `minRate` parameter passed to the swap function based on an external price feed and DEX's liquidity. Implement fee delegation to prepare for the application's launch.~~ | [https://github.com/vearnfi/mathematical_analysis/blob/main/README.md](https://github.com/vearnfi/mathematical_analysis/blob/main/README.md) [https://github.com/vearnfi/events-fetcher](https://github.com/vearnfi/events-fetcher) [https://github.com/vearnfi/firebase](https://github.com/vearnfi/firebase)
| 3 | Front End | Build upon the Milestone 1 specifications. Hire a designer to enhance the front-end interface aesthetics and UX. Add an input field for users to specify the minimum amount of VTHO they wish to retain in their account after the swap. | [https://github.com/vearnfi/client](https://github.com/vearnfi/client)
| 4 | Community | Make the application available for users to try on the testnet and actively gather feedback from the community. | [https://vearn.finance/](https://vearn.finance/) [https://discord.gg/KSE8RaF8Ft](https://discord.gg/KSE8RaF8Ft)

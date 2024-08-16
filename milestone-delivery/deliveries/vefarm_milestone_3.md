# Milestone Delivery :mailbox:

> Only the GitHub account, which is responsible for the pull request of the accepted application is allowed to submit milestones. Don't remove any of the mandatory parts presented in bold letters or as headlines!

**The Ethereum address has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](../).**

* **PR Link:** [VeChain grant proposal - VeFarm #161](https://github.com/vechain/grant-program/pull/161)
* **Milestone Number:** 3

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
9. [vexchange wrapper](https://github.com/vearnfi/vex-wrapper): A wrapper around the Vexchange contract exposing the original uniswap V2 interface. In this way we can use the same ABI for both Verocket and Vexchange, simplifying the code.


| Number | Deliverable | Specification | Link |
|-|-|-|-|
| 0a.| License | MIT(*) |
| 0b. | Documentation | Provide comprehensive inline documentation of the code and create a basic tutorial that demonstrates interaction with the deployed smart contract. | [https://github.com/vearnfi/contracts/blob/main/README.md](https://github.com/vearnfi/contracts/blob/main/README.md)
| 0c. | Testing Guide | Ensure proper unit test coverage (e.g., 90%) for the code functionality and robustness. Document the steps to run these tests in a testing guide. | Please, refer to the testing section inside each repository.
| 0d. | User Guide | Prepare a user guide or demo video showcasing the implemented features ~~as well as a Gitbook~~. | [https://medium.com/@vearnfi/grow-your-vet-balance-with-vearn-finance-a227d2b02de9](https://medium.com/@vearnfi/grow-your-vet-balance-with-vearn-finance-a227d2b02de9)
| 1 | Smart Contracts | Enhance the VeFarm smart contract based on feedback received in the previous phase. Deploy the contract to the mainnet and conduct real-world testing before launch. Open source the smart contract and upload the ABI to the B32 repository. [B32](https://github.com/VeChain/b32). | [B32 PR](https://github.com/vechain/b32/pull/66). A [Roles](https://github.com/vearnfi/contracts/blob/main/contracts/Roles.sol) contract was created to handle user roles outside the [Trader](https://github.com/vearnfi/contracts/blob/main/contracts/Trader.sol) contract. Additionally, a [Vexchange Wrapper](https://github.com/vearnfi/vex-wrapper) contract was developed to allow the Trader contract to interact with Vexchange using the original Uniswap V2 interface.
| 2 | Backend | Update the swap algorithm and overall backend architecture and infrastructure based on insights gained in the previous stage. Deploy a production environment ~~and enable fee delegation functionality~~ (Fee delegation will be postponed for a latter stage). | [https://github.com/vearnfi/firebase](https://github.com/vearnfi/firebase)
| 3 | Front End | Align with backend updates. Improve the frontend interface and user experience accordingly. | A designer was hired to improve the UX and UI.  [https://vearn.finance/](https://vearn.finance/) [https://testnet.vearn.finance/](https://testnet.vearn.finance/)
| 4 | Community | Engage with the community and launch the application into production. Gather feedback and promptly address any identified issues.| [https://vearn.finance/](https://vearn.finance/) [https://testnet.vearn.finance/](https://testnet.vearn.finance/) [https://discord.gg/KSE8RaF8Ft](https://discord.gg/KSE8RaF8Ft)

(*) The VeFarm smart contract will be open source, while the frontend and backend will remain closed source.

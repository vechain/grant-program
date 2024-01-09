# Milestone Delivery :mailbox:

> Only the GitHub account, which is responsible for the pull request of the accepted application is allowed to submit milestones. Don't remove any of the mandatory parts presented in bold letters or as headlines!

**The Ethereum address has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](../).**

- **PR Link:** https://github.com/vechain/grant-program/pull/132
- **Milestone Number:** 1

Please provide a list of all deliverables of the milestone extracted from the initial application and a link to the deliverable itself. Ideally all links inside the below table should include a commit hash, which should be used for testing.

| Number | Deliverable                           | Specification                                                                                                                                                                                                                    | Link                                                                                                                  |
| ------ | ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| 0a.    | Documentation                         | We will provide simple documentation for each contract, explaining their main functions nad their roles.                                                                                                                         | https://github.com/SayNode/FondueSwap/tree/master/documentation Commit Hash: 0f67785c83fdb3036d69b66403561ad353c92af1 |
| 0b.    | Testing Guide                         | The code will have proper unit-test coverage (e.g. 90%) to ensure functionality and robustness. We will describe how to run both the Brownie and Vechain testnet tests.                                                          | https://github.com/SayNode/FondueSwap/tree/master/documentation Commit Hash: 0f67785c83fdb3036d69b66403561ad353c92af1 |
| 1a.    | Smart Contracts: Development          | We will develop smart contracts that will deal with pool creating and indexing (Pool Factory contract) and with the pool operations (swaps, position setting, checking and changing).                                            | https://github.com/SayNode/FondueSwap/tree/master/contracts Commit Hash: 86101b123dbb2dc0f7360f88fc49295469e0a5f4     |
| 1b.    | Smart Contracts: Testing with Brownie | We will create several tests in Brownie. Because brownie allows us to run a mock up of the Ethereum blockchain and simulate the passage of time, we can run several tests in a matter of seconds, making it easier for debugging | https://github.com/SayNode/FondueSwap/tree/master/tests Commit Hash: 86101b123dbb2dc0f7360f88fc49295469e0a5f4         |
| 1c.    | Smart Contracts: Testing in Vechain   | We will replicate all the Brownie tests but with <s>regular Python scripts, using the thor-requests library and</s> the testnet. This way we can make sure there is no functionality loss between blockchains.                   | https://github.com/SayNode/FondueSwap/tree/master/tests_vechain Commit Hash: 0f67785c83fdb3036d69b66403561ad353c92af1 |

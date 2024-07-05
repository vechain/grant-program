# Milestone Delivery :mailbox:

> Only the GitHub account, which is responsible for the pull request of the accepted application is allowed to submit milestones. Don't remove any of the mandatory parts presented in bold letters or as headlines!

**The Ethereum address has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](../).**

* **PR Link:** [VeChain grant proposal - VeFarm #161](https://github.com/vechain/grant-program/pull/161)
* **Milestone Number:** 1

Please provide a list of all deliverables of the milestone extracted from the initial application and a link to the deliverable itself. Ideally all links inside the below table should include a commit hash, which should be used for testing.

**Overview:** The project has been split into several repositories:

1. [client](https://github.com/vearnfi/client): Frontend for the vearn protocol. It is responsible for interacting with the Energy and Trader contracts and making calls to the backend.
2. [backend/firebase](https://github.com/vearnfi/firebase): Serverless backend responsible for storing all data related to the vearn protocol, fetching events and calling the `swap` function on the `Trader` contract.
3. [contracts](https://github.com/vearnfi/contracts): Smart contracts associated with the vearn protocol.

#### Milestone 1 — POC

| Number | Deliverable | Specification | Link
|-|-|-|-|
| 0 | Smart Contract | Create a non-upgradable smart contract that provides a `swap` function. The function will require the following parameters: `account` (payable address - target account), `amountIn` (uint256 - VTHO amount to be swapped), and `minRate` (uint256 - minimum accepted exchange rate). When invoked, the smart contract will transfer VTHO tokens from the user's balance to the contract's balance. It will then approve the DEX contract to spend the specified amount of tokens (no fees will be deducted in this milestone). Finally, the contract will call the `swapExactTokensForETH` function on the DEX contract to perform the swap, with the target account as the destination address. After the trade is completed, the contract will emit a `Swap` event to log relevant information, including the `account`, `amountIn`, and `amountOut` (uint256 - VET amount received after the swap). It is worth mentioning that the contract is designed to be non-custodial, ensuring that users' funds stay in their accounts until the swap function is executed. | [https://github.com/vearnfi/contracts/commit/6d70c430331e1d4de899517a63d6ead927d480d2](https://github.com/vearnfi/contracts/commit/6d70c430331e1d4de899517a63d6ead927d480d2)
| 1 | Backend | Develop a backend service to periodically retrieve the `Approval` events emitted by the VTHO contract. This service will store the accounts that have approved the VeFarm contract for token spending. For these approved accounts, implement a job that periodically fetches the account balance and triggers the `swap` function on the VeFarm contract based on a simple strategy: whenever the user's balance reaches 5 VTHO (keeping the `minRate` constant). The backend service will listen to the `Swap` events emitted by the VeFarm contract after the trade is completed and store relevant information in the database, including the VTHO input amount, VET output amount, and transaction ID. Track basic statistics such as the total number of accounts, transaction count, and the amounts of VTHO and VET being swapped. Additionally, provide an endpoint to query the statistics and retrieve the list of transactions associated with a specific account. | [https://github.com/vearnfi/firebase/commit/c62d37f026451a5c175754ae31aea752e1f7e653](https://github.com/vearnfi/firebase/commit/c62d37f026451a5c175754ae31aea752e1f7e653)
| 2 | Front End | Build a basic front-end interface that allows users to log in, view their current balance, authorize the VeFarm contract to spend their VTHO tokens, revoke approval, and access a list of past transactions. | [https://github.com/vearnfi/client/commit/bc0b738a94eb2d57662edf90135fb00e55fb85d8](https://github.com/vearnfi/client/commit/bc0b738a94eb2d57662edf90135fb00e55fb85d8)

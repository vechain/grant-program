# Milestone Delivery :mailbox:

**The Ethereum address has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](../).**  

* **PR Link:** https://github.com/vechain/grant-program/pull/46 
* **Milestone Number:** 1


The basic functionality on the contract part is now implemented. Deployment and Tests are available. The jest Tests are added below the table. For testing purpose the deployment addresses and a (Work-In-Progress) TestNet-Web-UI are listed as well.


| Number | Deliverable | Link | Notes |
| ------------- | ------------- | ------------- |:-----------: |
| 1.0 | Setup | Setup Project including a CI/CD-Pipeline that auto-deploys to Test- and MainNet after running Unit-Tests | ✓
| 1.1 | NFT-Contract | Create Sponsorships as NFT with full ERC/VIP Support | ✓
| 1.2 | Token-Configuration | Add functionality to for configuration of signing-parameters in the tokens | ✓
| 1.3 | Signing-Confirmation | Confirm Signing within the contract (incl. calling reference contracts if signing is supported) | ✓
| 1.4 | Deposit / Withdraw | Ability to deposit and withdraw VET/VTHO linked to a Token | ✓
| 1.5 | Key/Value-Store | Ability to store configuration values without upgrading the contract (EIP-725) | ✓
| 1.6 | Self-Init | Automatically self-init contract to sponsor itself with the first sponsorship | ✓
| 1.7 | Versioning | Tokens can be linked and verification run with different contract variants/versions to support new and different features over time | ✓
| 1.8 | Example-Snippets | Write examples and documentation for other developers to implement the interface for contract interaction | ✓   https://testnet.vechain.energy/#/docs/contracts

## Unit-Test-Report

Results of the jest tests:

```
$ yarn test
yarn run v1.22.17
$ hardhat test:jest
✅ Generated documentation for 40 contracts
 PASS  src/Sponsorship.VIP-181.test.js
  1.1 Sponsorship, ERC-721 / VIP-181 (based on OpenZeppelin ERC-721)
    Basics
      ✓ supports name() (606 ms)
      ✓ supports symbol() (151 ms)
    balanceOf(address)
      ✓ returns count of owned tokens (175 ms)
      ✓ respects burned tokens (154 ms)
      ✓ returns 0 for unknown addresses (92 ms)
    ownerOf(address)
      ✓ supports ownerOf(tokenId) (102 ms)
      ✓ fails for unknown tokenId (116 ms)
    tokenOfOwnerByIndex(address, index)
      ✓ supports tokenOfOwnerByIndex(address, index) (112 ms)
      ✓ fails for invalid index (79 ms)
    tokenByIndex(index)
      ✓ supports tokenByIndex(index) (94 ms)
      ✓ fails for invalid index (78 ms)
    totalSupply()
      ✓ supports totalSupply() (100 ms)
      ✓ respects burned tokens in count (112 ms)
    burn(tokenid)
      ✓ supports burn(tokenId) (96 ms)
      ✓ rejects burn(tokenId) for none-token-owners (88 ms)
    transferFrom(from, to, tokenId)
      ✓ supports ownership transfer (95 ms)
      ✓ fails for none-owners (90 ms)
    approve(spender, tokenId)
      ✓ allows another user to transfer ownership (99 ms)
      ✓ still allows owner to transfer (124 ms)
    setApprovalForAll(operator, approved)
      ✓ allows another user to transfer ownership of all tokens (115 ms)
      ✓ setApprovalForAll(operator, false) removes previous approval (94 ms)
    isApprovedForAll(owner, operator)
      ✓ returns false by default (70 ms)
      ✓ returns true when set (79 ms)
      ✓ returns false when set (80 ms)

PASS  src/Sponsorship/Configuration.test.js
  1.2 + 1.7 Sponsorship Configuration
    configure contract address
      ✓ supports setContractFor(address, tokenId) (638 ms)
      ✓ default value is an empty address "0x0000000000000000000000000000000000000000" (169 ms)
      ✓ supports contractOf(tokenId) (142 ms)
      ✓ fires event "ContractChanged" with new information on update (143 ms)
      ✓ rejects updates from users that are not owner of the token (135 ms)
    configure allowed senders
      addAllowedSenderFor(address, tokenId)
        ✓ supports addAllowedSenderFor(address, tokenId) (110 ms)
        ✓ lists added senders in allowedSendersFor(tokenId) (115 ms)
        ✓ supports multiple adds (112 ms)
        ✓ rejects updates from users that are not owner of the token (91 ms)
      removeAllowedSenderFor(address, tokenId)
        ✓ supports removeAllowedSenderFor(address, tokenId) (87 ms)
        ✓ unlists senders in allowedSendersFor(tokenId) (104 ms)
        ✓ rejects updates from users that are not owner of the token (88 ms)
      allowedSendersFor(tokenId)
        ✓ supports allowedSendersFor(address, tokenId) (88 ms)
        ✓ is empty by default (85 ms)
    configure allowed recipients
      addAllowedRecipientFor(address, tokenId)
        ✓ supports addAllowedRecipientFor(address, tokenId) (88 ms)
        ✓ lists added Recipients in allowedRecipientsFor(tokenId) (89 ms)
        ✓ supports multiple adds (95 ms)
        ✓ rejects updates from users that are not owner of the token (84 ms)
      removeAllowedRecipientFor(address, tokenId)
        ✓ supports removeAllowedRecipientFor(address, tokenId) (85 ms)
        ✓ unlists Recipients in allowedRecipientsFor(tokenId) (89 ms)
        ✓ rejects updates from users that are not owner of the token (80 ms)
      allowedRecipientsFor(tokenId)
        ✓ supports allowedRecipientsFor(address, tokenId) (84 ms)
        ✓ is empty by default (78 ms)
    configure different versions of verification workflows
      ✓ supports setVersionFor(version, tokenId) (80 ms)
      ✓ returns the current version with versionOf(tokenId) (86 ms)
      ✓ fires event "VersionChanged" with new information on update (115 ms)
      ✓ defaults to version 0 (74 ms)
      ✓ rejects updates from users that are not owner of the token (76 ms)

 PASS  src/Sponsorship.Signing.test.js
  1.3 + 1.7 Sponsorship, Decision-Finding
    v0
      canSponsorTransactionForToken(sender, recipient, data, tokenId) for verification
        ✓ supports canSponsorTransactionForToken(sender, recipient, data, tokenId) (1200 ms)
        ✓ accepts a sender in allowedSendersFor(tokenId) (189 ms)
        ✓ accepts a recipient in allowedRecipientsFor(tokenId) (147 ms)
        ✓ accepts to work with 0x as recipient (146 ms)
        ✓ rejects if a transaction is not in sender OR recipient (111 ms)
        ✓ calls correctly canSponsorTransactionFor(sender, recipient, data) on configured contractAddress and returns the false value (125 ms)
        ✓ fails to call canSponsorTransactionFor(sender, recipient, data) for non-contract-addresses  (128 ms)
        ✓ returns false on contracts that do not correctly support canSponsorTransactionFor(sender, recipient, data)  (123 ms)
        calls correctly canSponsorTransactionFor(sender, recipient, data) on configured contractAddress and returns the true value
          ✓ works with sender (150 ms)
          ✓ works with recipient (139 ms)
          ✓ works with data (124 ms)
    unsupported versions
      ✓ returns false for unsupported versions (132 ms)

 PASS  src/Sponsorship.test.js
  1.4 + 1.6 Sponsorship
    Initialize
      ✓ identifies as version #1 (632 ms)
      ✓ mints an initial token with contract owner as owner (165 ms)
      ✓ configures contract address on initial token (126 ms)
    Minting
      ✓ supports mintSponsorship(title) (114 ms)
      ✓ emits an event Transfer on mint (107 ms)
      ✓ auto increments token ids (119 ms)
      ✓ assigns ownership of sponsorship to msg.sender (99 ms)
    canSponsorTransactionFor(sender, recipient, data) to support own sponsorship API
      ✓ supports all transactions with to = contract.address (91 ms)
      ✓ supports all transactions with to = any token owner (87 ms)
      ✓ supports all data-transactions with to = any token owner (87 ms)
      ✓ defaults to false for other transactions (76 ms)
      ✓ returns false if data is something else (75 ms)
    requestWithdrawBalanceFor(tokenId)
      ✓ emits event WithdrawBalance(tokenId) (87 ms)
      ✓ accepts only token owner (104 ms)
    Withdraw trapped funds
      ✓ restricts withdrawTokenTo(token, to) to owner (113 ms)
      ✓ restricts withdrawBalanceTo(to) to owner (79 ms)
      ✓ transfers whole balance with withdrawBalanceTo(to) (82 ms)
      ✓ supports withdrawTokenTo(token, to) (113 ms)

 PASS  src/Sponsorship/KeyValue.test.js
  1.5 Sponsorship
    Key/Value Store (inspired by EIP-725Y)
      ✓ supports setDataFor(keys[], values[], tokenId) (1179 ms)
      ✓ rejects setDataFor(keys[], values[], tokenId) for none-token-owner (188 ms)
      ✓ supports getDataFor(keys[], tokenId) and returns set values (152 ms)
      ✓ returns empty strings for none-set keys on getDataFor(keys[], tokenId)  (145 ms)
      ✓ emits DataChanged(key, value, tokenId) for each set value (120 ms)

 PASS  src/helper/ExampleSponsored.test.js
  ExampleSponsored
    ✓ supports canSponsorTransactionFor(sender, recipient, data) returns true for owner (993 ms)
    ✓ supports canSponsorTransactionFor(sender, recipient, data) returns false otherwise (50 ms)
    ✓ supports canSponsorTransactionFor(sender, recipient, data) with ERC token transfer in data (52 ms)
    ✓ does not crash on empty data calls (71 ms)
    ✓ does not crash on invalid data calls (49 ms)

 PASS  src/EnergyProxy.test.js
  EnergyProxy
    ✓ can be deployed (548 ms)
    ✓ proxies all requests to implementation (155 ms)
    ✓ calls initializer of implementation (142 ms)
    ✓ supports upgrade while keeping data (169 ms)
    ✓ rejects upgradeTo from none-owner (156 ms)
    ✓ supports owner change (174 ms)

Test Suites: 7 passed, 7 total
Tests:       98 passed, 98 total
Snapshots:   0 total
Time:        4.976 s, estimated 5 s
Ran all test suites.
✨  Done in 9.41s.
```

### TestNet

* Proxy: 
https://explore-testnet.vechain.org/accounts/0xd4167930fc4a547ff71ccbd0b067d8a30c0f2d3c
* Implementation: https://explore-testnet.vechain.org/accounts/0xea542d8d4742d638f1156b8dc4c7a20f80eff024
* The TestNet-Contract can managed using https://testnet.vechain.energy

### MainNet

* Proxy: 
https://explore.vechain.org/accounts/0xcd15c3b9b4898cdbb183dc820017b969430bb18e
* Implementation: https://explore.vechain.org/accounts/0xb6307e36d76b9164c620ef60f5875efdfb36e59a


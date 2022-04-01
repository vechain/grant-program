# Milestone Delivery :mailbox:

**The Ethereum address has been filled out correctly for this milestone and the delivery is according to the official [milestone delivery guidelines](../).**  

* **PR Link:** https://github.com/vechain/grant-program/pull/46 
* **Milestone Number:** 2


The basic functionality on the backend part is now implemented. Deployment and Tests are available. The jest Tests are added below the table. For testing purpose the deployment links and a (Work-In-Progress) TestNet-Web-UI are listed as well.


| Number | Deliverable | Link | Notes |
|-|-|-|-
| 2.0 | Setup | Setup Project including a CI/CD-Pipeline that auto-deploys to Staging, Development and Production URLs | ✓
| 2.1 | Wallet | Wallet Management for each Token to use for Co-Signing | ✓
| 2.2 | Signing-Confirmation | Verify Requests against Contract | ✓
| 2.3 | Co-Signing | Co-Signing of transactions using the Wallet for each Token | ✓
| 2.4 | Pre-Check | Allow to pre-validate a transaction before submitting it for Co-Signing | ✓
| 2.5 | Deposit / Withdraw | Ability to handle VET/VTHO deposits and withdraw the funds from the managed wallets | ✓
| 2.6 | Logging | Logging of signing requests (without IP-Address by default) linked to each Token and automatic deletion | ✓ retention is configured at CloudWatch
| 2.7 | Sessions | An Auth-Workflow that handles web3auth and Sync2 as Session-Management (by issueing a Token that is signed by the user and verified on subsequent requests) | ✓
| 2.8 | Log-Access | Provide access to Logs with a filter and query parameters and the ability to download | ✓


## Unit-Test-Report

Results of the jest tests:

```
$ yarn test --coverage  --verbose
yarn run v1.22.17

 PASS  modules/getWallet.test.js
  2.1 Wallet handling
    ✓ generates a new wallet for given token (385 ms)
    ✓ rejects for missing tokenId (5 ms)
    ✓ supports tokenId #0 (325 ms)
    ✓ returns { address, privateKey } (321 ms)
    ✓ returns a different wallet for each token (628 ms)
    ✓ returns the same wallet on subsequent calls of the same tokenId (352 ms)
    ✓ stores the wallet on the expected location (319 ms)

 PASS  routes/address/index.test.js
  2.1 POST /address/:tokenId – retrieve signing address for token
    ✓ passes tokenId to getWallet() (358 ms)
    ✓ updates signer in contract (49 ms)
    ✓ responds with { tokenId, address } (37 ms)


 PASS  modules/contract/canSponsorTransactionForToken.test.js
  2.2 canSponsorTransactionForToken({ origin, transaction, tokenId, connex })
    ✓ connects to contract address using connex.thor.account(address) (1 ms)
    ✓ calls canSponsorTransactionForToken(origin, to, data, tokenId) for each transaction clause
    ✓ passes clause data correctly to contract call
    ✓ uses address(0) for validation if to is missing
    ✓ throws if contract does not respond with true (8 ms)
    ✓ uses the correct ABI definition for the function call

 PASS  routes/sponsor/index.test.js
  2.3 + 2.6 POST /by/:tokenId – transaction signing
    ✓ requires "raw" (159 ms)
    ✓ requires "origin" (1 ms)
    ✓ passes tokenId to getWallet() (275 ms)
    ✓ responds with { signature, address } (107 ms)
    ✓ responds with { error } if signing is not supported (1 ms)
    ✓ signs with the wallet assigned to tokenId (110 ms)
    ✓ calls canSponsorTransactionForToken({ origin, transaction, tokenId, connex }) for verification (105 ms)
    ✓ rejects signing if canSponsorTransactionForToken() throws
    Logging
      ✓ logs "tokenId" for signed transactions (106 ms)
      ✓ logs "origin" for signed transactions (104 ms)
      ✓ logs "signature" for signed transactions (105 ms)
      ✓ logs "address" for signed transactions (105 ms)
      ✓ logs "raw" for signed transactions (104 ms)
      ✓ logs errors with "tokenId" for rejected transactions (1 ms)
      ✓ logs errors with "origin" for rejected transactions (1 ms)
      ✓ logs errors with "raw" for rejected transactions
      ✓ logs errors with "rejected" for rejected transactions (1 ms)
      ✓ logs errors with "error" for rejected transactions
      ✓ logs errors with occured error for rejected transactions (1 ms)

 PASS  routes/sponsor/test/index.test.js
  2.4 POST /by/:tokenId/test – pre-validate transaction signing
    ✓ requires "raw" (154 ms)
    ✓ requires "origin" (1 ms)
    ✓ responds with "success" if signing is supported (289 ms)
    ✓ responds with the delegating address in "delegator" (75 ms)
    ✓ responds with the energy balance of the delegator in "energy" as a number (95 ms)
    ✓ responds with "errors[]" if signing is not supported (69 ms)
    ✓ responds with success false if signing is not supported (68 ms)
    ✓ responds with currently configured network-type (67 ms)
    ✓ calls canSponsorTransactionForToken({ origin, transaction, tokenId, connex }) for verification (70 ms)

 PASS  modules/eventHandler/withdrawBalance.test.js
  2.5 eventListener/eventHandler/WithdrawBalance
    ✓ looks up the correct wallet for the given tokenId (79 ms)
    ✓ sends a transaction with full VET Balance and full VTHO Balance (70 ms)

 PASS  routes/auth/tokens.test.js
  2.7 POST /tokens – get token for signing identity
    ✓ returns a token (183 ms)
    ✓ returns a different token on each request (6 ms)

 PASS  modules/jwks/index.test.js
  2.7 JWKS
    ✓ exports "get" (1 ms)
    ✓ exports "sign"
    get
      ✓ returns a JWKS object on get() (62 ms)
      ✓ returns the JWKS object on subsequent calls of get()
    sign
      ✓ signs the given payload (3 ms)
      ✓ signs with the JWKS returned by get() (11 ms)

 PASS  modules/jwks/generate.test.js
  2.7 JWKS/generate
    ✓ generates a new JWKS file at the given filepath (91 ms)
    ✓ writes a valid JWKS (77 ms)

 PASS  modules/sessionValidation/index.test.js
  2.7 module
    ✓ exports Session.verify(certificaten, jwks) as function

 PASS  modules/jwks/get.test.js
  2.7 JWKS/get
    ✓ returns a JWKS from a given filename (32 ms)

 PASS  routes/jwks/index.test.js
  2.7 GET /jwks – json web key set
    ✓ returns a list of keys (170 ms)

 PASS  routes/auth/authTest.test.js
  2.7 GET /auth/test – test auth header
    ✓ identifies signer correctly when token is correctly signed (750 ms)
    ✓ fails for invalid signed session headers (463 ms)

 PASS  routes/logs/index.test.js (5.223 s)
  2.8 GET /logs/:tokenId – get previous sponsorship requests
    ✓ rejects if requestee is not token owner (926 ms)
    ✓ fails for invalid signed session headers (480 ms)
    ✓ gets CloudWatch Logs filtered by tokenId (471 ms)
    ✓ returns log data (474 ms)
    ✓ returns event log in CSV format if format=csv is given (463 ms)
    ✓ filters with 28 days by default (460 ms)
    ✓ limits filter time to 28 days (456 ms)
    ✓ support "days" as filter (470 ms)

 PASS  routes/status.test.js
  GET /status – availability endpoint
    ✓ returns statusCode 200 (150 ms)
    ✓ returns an object for future verifiation

 PASS  routes/index.test.js
  GET / – placeholder homepage
    ✓ returns statusCode 200 (162 ms)
    ✓ returns a placeholder content

 PASS  test/connex.test.js
  plugins/connex
    ✓ provides a connex instances (144 ms)
    ✓ provides the same connex instance every time (2 ms)

 PASS  modules/eventHandler/Transfer.test.js
  eventListener/eventHandler/Transfer
    ✓ looks up the correct wallet for the given tokenId (76 ms)
    ✓ sends a transaction with setSignerFor(address, tokenId) using the tokens wallet address (70 ms)

 PASS  modules/eventHandler/getFilter.test.js
  eventListener/filters
    ✓ configures an event filter for "WithdrawBalance"
    ✓ configures an event filter for "Transfer"

 PASS  modules/eventListener.test.js
  eventListener
    ✓ starts a loop handling every block (11 ms)
    ✓ filters events on each block (12 ms)
    ✓ calls eventHandler with "decoded" for every event (22 ms)

 PASS  modules/contract/setSignerFor.test.js
  contract/setSignerFor
    ✓ uses the correct contract (1 ms)
    ✓ throws if tokenId is not known (validated by ownerOf) (6 ms)
    ✓ returns no clauses if signer is the same (validated against signerOf)
    ✓ returns correct clause with given arguments

-----------------------------------|---------|----------|---------|---------|-------------------------------
File                               | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s             
-----------------------------------|---------|----------|---------|---------|-------------------------------
All files                          |    77.1 |    97.36 |      90 |    77.1 |                               
 backend                           |     100 |      100 |     100 |     100 |                               
  app.js                           |     100 |      100 |     100 |     100 |                               
 backend/modules                   |   44.02 |      100 |      50 |   44.02 |                               
  eventListener.js                 |     100 |      100 |     100 |     100 |                               
  getCloudWatchLog.js              |    9.09 |      100 |       0 |    9.09 | 4-33                          
  getWallet.js                     |     100 |      100 |     100 |     100 |                               
  sendTransaction.js               |    6.41 |      100 |       0 |    6.41 | 5-56,58-78                    
  verifyAuthorizationHeader.js     |     100 |      100 |     100 |     100 |                               
 backend/modules/contract          |     100 |      100 |     100 |     100 |                               
  canSponsorTransactionForToken.js |     100 |      100 |     100 |     100 |                               
  setSignerFor.js                  |     100 |      100 |     100 |     100 |                               
 backend/modules/eventHandler      |     100 |      100 |     100 |     100 |                               
  Transfer.js                      |     100 |      100 |     100 |     100 |                               
  getFilter.js                     |     100 |      100 |     100 |     100 |                               
  withdrawBalance.js               |     100 |      100 |     100 |     100 |                               
 backend/modules/jwks              |     100 |      100 |     100 |     100 |                               
  generate.js                      |     100 |      100 |     100 |     100 |                               
  get.js                           |     100 |      100 |     100 |     100 |                               
  index.js                         |     100 |      100 |     100 |     100 |                               
  sign.js                          |     100 |      100 |     100 |     100 |                               
 backend/modules/sessionValidation |    90.9 |       50 |     100 |    90.9 |                               
  index.js                         |     100 |      100 |     100 |     100 |                               
  verify.js                        |   89.47 |       50 |     100 |   89.47 | 11-12                         
 backend/plugins                   |   76.47 |      100 |     100 |   76.47 |                               
  CloudWatch.js                    |     100 |      100 |     100 |     100 |                               
  connex.js                        |     100 |      100 |     100 |     100 |                               
  sendTransaction.js               |   25.92 |      100 |     100 |   25.92 | 7-26                          
  sequelize.js                     |     100 |      100 |     100 |     100 |                               
 backend/routes                    |   29.62 |      100 |     100 |   29.62 |                               
  index.js                         |     100 |      100 |     100 |     100 |                               
  playground.js                    |   13.63 |      100 |     100 |   13.63 | 7-29,32-55,58-73,76-92,95-109 
 backend/routes/address            |   91.42 |    66.66 |     100 |   91.42 |                               
  index.js                         |   91.42 |    66.66 |     100 |   91.42 | 13-15                         
 backend/routes/auth               |     100 |      100 |     100 |     100 |                               
  authTest.js                      |     100 |      100 |     100 |     100 |                               
  tokens.js                        |     100 |      100 |     100 |     100 |                               
 backend/routes/jwks               |     100 |      100 |     100 |     100 |                               
  index.js                         |     100 |      100 |     100 |     100 |                               
 backend/routes/logs               |     100 |      100 |     100 |     100 |                               
  index.js                         |     100 |      100 |     100 |     100 |                               
 backend/routes/sponsor            |     100 |      100 |     100 |     100 |                               
  index.js                         |     100 |      100 |     100 |     100 |                               
 backend/routes/sponsor/test       |     100 |      100 |     100 |     100 |                               
  index.js                         |     100 |      100 |     100 |     100 |                               
-----------------------------------|---------|----------|---------|---------|-------------------------------
Test Suites: 21 passed, 21 total
Tests:       86 passed, 86 total
Snapshots:   0 total
Time:        20.071 s
Ran all test suites.
Force exiting Jest: Have you considered using `--detectOpenHandles` to detect async operations that kept running after all tests finished?
✨  Done in 20.53s.

```


### TestNet

* Backend: https://sponsor-testnet.vechain.energy/documentation
* The TestNet-Backend can managed using https://testnet.vechain.energy

### MainNet

* Backend: https://sponsor-mainnet.vechain.energy/documentation

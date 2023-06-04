
# Milestone Delivery :mailbox:

**The Ethereum address has been filled out correctly for this milestone, and the delivery is according to the official [milestone delivery guidelines](../).**

* **PR Link:** https://github.com/vechain/grant-program/pull/115
* **Milestone Number:** 2


## Milestone 2

The Virtual Node is running on CloudFlare and accesses all known nodes:

| Number | Deliverable | Link | Notes |
|--------|-------------|------|-------|
| 2.0 | Proxy | Unit Test Report shown below |  |
| 2.1 | TestNet | https://node-testnet.vechain.energy/blocks/best |  |
| 2.2 | MainNet | https://node-mainnet.vechain.energy/blocks/best |  |

The generic behavior can be explained by:

* try node to fetch data from a node until a successful response is returned
* verify sync-status when switching nodes or during `best` block requests

```shell
$ jest --verbose
 PASS  src/modules/verifyNodeSsyncStatus.test.ts
  verifyNodeSyncStatus(response, origin)
    ✓ returns response if timestamp is recent (9 ms)
    ✓ throws error if timestamp is too old (3 ms)

 PASS  src/modules/verifyResponseStatus.test.ts
  verifyResponseStatus(response)
    ✓ throws error for redirects (11 ms)
    ✓ returns response for tx-related errors (1 ms)
    ✓ throws error for other errors >=400 (1 ms)

 PASS  src/getNodeByType.test.ts
  getNodeByType(type)
    ✓ supports node type "test" (1 ms)
    ✓ supports node type "main"
    ✓ throws if unknown network type is requested (3 ms)
    ✓ returns a different URL each time it is called
    ✓ cycles through all available URLs before repeating (1 ms)

 PASS  src/modules/generateTranportHeaders.test.ts
  generateTransportHeaders(request)
    ✓ returns expected headers (9 ms)
    ✓ returns only defined headers (1 ms)
    ✓ returns empty object if request has no headers

 PASS  src/modules/generateReturnHeaders.test.ts
  generateReturnHeaders(response, origin)
    ✓ returns expected headers (7 ms)
    ✓ returns origin node url in "x-node-url"
    ✓ defaults "access-control-max-age" to 86400
    ✓ defaults "access-control-allow-origin" to "*" (1 ms)
    ✓ returns only defined headers
    ✓ returns default headers if response has no headers

 PASS  src/retryFetch.test.ts
  retryFetch
    ✓ returns a successful response (10 ms)
    ✓ re-uses the last successful node (1 ms)
    ✓ detects network by hostname (1 ms)
    ✓ retries with another node on error (104 ms)
    ✓ skips another node if it not up-to-date (219 ms)
    ✓ does a node-sync-check on calling /blocks/best (103 ms)
    ✓ returns error if node list is exhausted (2040 ms)

Test Suites: 6 passed, 6 total
Tests:       26 passed, 26 total
Snapshots:   0 total
Time:        3.64 s, estimated 4 s
Ran all test suites.
✨  Done in 4.37s.
```

# Milestone Delivery :mailbox:

**The Ethereum address has been filled out correctly for this milestone, and the delivery is according to the official [milestone delivery guidelines](../).**

* **PR Link:** https://github.com/vechain/grant-program/pull/214
* **Milestone Number:** 1

## Milestone 1


| Number | Deliverable | Link | Notes |
|-|-|-|-|
| 1.1 | Contract | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/contracts |
| 1.2 | TestNet | https://explore-testnet.vechain.org/accounts/0xdccaabd81b38e0deef4c202bc7f1261a4d9192c6
| 1.3 | MainNet | https://explore.vechain.org/accounts/0x49ec7192bf804abc289645ca86f1ed01a6c17713


**Contract Test Report**

```shell
 PASS  contracts/Oracle.test.js (6.449 s)
  Oracle 
    Oracle Contract "oracleV1"
      getLatestValue(id)
        ✓ returns (value, updatedAt) (1269 ms)
      updateValue(id, newValue, newTimestamp)
        ✓ rejects non-reporter calls (209 ms)
        ✓ stores input correctly (133 ms)
        ✓ accepts multiple ids (152 ms)
        ✓ updates values correctly (137 ms)
        ✓ emits ValueUpdate(bytes32 id, uint256 value, uint64 updatedAt) (126 ms)
      updateValueWithProof(message, extraData, signedFor)
        ✓ stores input correctly (227 ms)
        ✓ rejects invalidly signed input (218 ms)
        ✓ rejects timestamps in the past (233 ms)
        ✓ rejects timestamps 30m in the future (225 ms)
      isReporter(address)
        ✓ returns true if user is a current reporter for the oracle (112 ms)
        ✓ returns false if the given address is not a reporter (115 ms)
    Oracle Contract "oracleV2"
      getLatestValue(id)
        ✓ returns (value, updatedAt) (120 ms)
      updateValue(id, newValue, newTimestamp)
        ✓ rejects non-reporter calls (142 ms)
        ✓ stores input correctly (127 ms)
        ✓ accepts multiple ids (126 ms)
        ✓ updates values correctly (122 ms)
        ✓ emits ValueUpdate(bytes32 id, uint256 value, uint64 updatedAt) (113 ms)
      updateValueWithProof(message, extraData, signedFor)
        ✓ stores input correctly (213 ms)
        ✓ rejects invalidly signed input (210 ms)
        ✓ rejects timestamps in the past (211 ms)
        ✓ rejects timestamps 30m in the future (209 ms)
      isReporter(address)
        ✓ returns true if user is a current reporter for the oracle (110 ms)
        ✓ returns false if the given address is not a reporter (112 ms)

 PASS  contracts/OracleAggregatorUpgradable.test.js (6.835 s)
  Aggregator 
    addSource(address)
      ✓ rejects non-admin calls (1493 ms)
      ✓ adds a new feed source (216 ms)
      ✓ supports multiple new new feed sources (219 ms)
    removeSource(address)
      ✓ rejects non-admin calls (234 ms)
      ✓ removes a feed source (198 ms)
    isSource(address)
      ✓ returns false by default (183 ms)
      ✓ returns true for added sources (188 ms)
      ✓ returns false for removed sources (190 ms)
    sources()
      ✓ returns the list of sources (186 ms)
    setIgnoreUpdatesOlderThan(seconds)
      ✓ rejects non-admin calls (232 ms)
      ✓ sets the ignoreUpdatesOlderThan correctly (186 ms)
    getLatestValue(id)
      ✓ returns (value, updatedAt) (203 ms)
      ✓ returns the average for even list of multiple sources (233 ms)
      ✓ returns newest timestamp for even list of multiple sources (223 ms)
      ✓ returns the median for odd list of multiple sources (253 ms)
      ✓ ignores sources with an updatedAt older than ignoreUpdatesOlderThan (234 ms)
      ✓ accepts sources with an updatedAt >= ignoreUpdatesOlderThan (235 ms)
      ✓ include all sources if ignoreUpdatesOlderThan is 0 (233 ms)

 PASS  contracts/OracleGasOptimized.test.js
  OracleV2 
    updateReporter(address)
      ✓ rejects non-reporter calls (1216 ms)
      ✓ gives access to the new reporter address (57 ms)
      ✓ removes access for previous reporter (38 ms)

 PASS  contracts/OracleUpgradable.test.js
  OracleV1 
    Proxy
      ✓ upgrade requires UPGRADER_ROLE (1375 ms)
    Decentralization
      ✓ highlights a preferred reporter for the next update (191 ms)
```

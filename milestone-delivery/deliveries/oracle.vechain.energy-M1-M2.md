
# Milestone Delivery :mailbox:

**The Ethereum address has been filled out correctly for this milestone, and the delivery is according to the official [milestone delivery guidelines](../).**

* **PR Link:** https://github.com/vechain/grant-program/pull/214
* **Milestone Number:** 1 - 7

## Milestone 1 - 7


| Number | Deliverable | Link | Notes |
|-|-|-|-|
| 1.1 | Contract | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/contracts |
| 1.2 | TestNet | https://explore.vechain.org/accounts/0x49ec7192bf804abc289645ca86f1ed01a6c17713
| 1.3 | MainNet | https://explore-testnet.vechain.org/accounts/0xdccaabd81b38e0deef4c202bc7f1261a4d9192c6
| 2.1 | Configuration | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter
| 2.2 | Data-Loading | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter 
| 2.3 | Data-Extraction | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter
| 2.4 | Update-Check | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter
| 2.5 | Update Oracle | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter
| 2.6 | Feed Activity | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter
| 3.1 | Value fetcher | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter/src/modules |
| 3.2 | Signer | https://github.com/vechain-energy/oracle.vechain.energy/blob/main/reporter/src/modules/signCcipRequest.ts |
| 3.3 | Deployment | https://oracle.vechain.energy/vet-usd |
| 4.1 | Application | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/statuspage |
| 4.2 | Deployment | https://status.oracle.vechain.energy/ |
| 5.1 | Documentation | https://docs.vechain.energy/vechain.energy/Oracles/ | find each combination in the menu as submenu item
| 5.2 | Snippets  | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/example-consumers |
| 5.3 | Self-Host-Instructions  | https://docs.vechain.energy/vechain.energy/Oracles/Self-Hosting/ |
| 6.1 | Multi-Reporter | https://github.com/vechain-energy/oracle.vechain.energy/blob/main/contracts/contracts/OracleAggregatorUpgradable.sol | has been moved into a separate contract
| 6.2 | Documentation | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/contracts#oracle-aggregator | isolated into the aggregator contract
| 7.0 | VTHO | no delivery required | has used ~1500 VTHO in the first two months of this year

**The Reporter API documentation is also available:**

- https://node.vechain.energy/doc/swagger-ui/?url=https://raw.githubusercontent.com/vechain-energy/oracle.vechain.energy/main/reporter/public/swagger.yml#/
- CCIP Requests can be tested manually `/{feedId}/resolver?sender={sender}&data={data}` endpoint in the swagger api


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


**Reporter Test Report**

```shell
$ yarn test --verbose
 PASS  src/modules/signCcipRequest.test.ts
  signCcipRequest({ request, config, report, env })
    ✓ signs the request correctly (36 ms)
    ✓ responds with (uint128 value, uint128 updatedAt, bytes32 feedId) (4 ms)

 PASS  src/modules/requiredUpdates.test.ts
  requiredUpdates(config, value)
    ✓ returns list of contracts that need updating (7 ms)
    ✓ returns empty list if no contracts need updating (3 ms)
  isUpdateRequired(config, value)
    ✓ requests last value & prefererd reporter from blockchain (1 ms)
    ✓ returns false if blockchain node could not handle data correctly (1 ms)
    ✓ returns true if contract reverts due missing data (1 ms)
    ✓ returns preferredReporter (2 ms)
    heartbeat
      ✓ returns true if last update is >= heartbeat interval (1 ms)
      ✓ returns false if age < heartbeat interval
    deviationPoints
      ✓ returns true if deviation >= configured value (4 ms)
      ✓ returns false if deviation < configured value (1 ms)

 PASS  src/modules/publishReport.test.ts
  publishReport({ contract, report, env })
    ✓ generates the correct transaction for updates (28 ms)
    ✓ uses fee delegation when delegationUrl is configured (16 ms)
    ✓ submits the signed transaction correctly (1 ms)
    ✓ returns raw text result from transaction submission (8 ms)

 PASS  src/modules/signTransaction.test.ts
  signTransaction(transaction, payload, privateKey)
    ✓ returns { signature, address } (87 ms)

 PASS  src/modules/fetchDataSources.test.ts
  fetchDataSources(config)
    ✓ loads data from each source (539 ms)
    ✓ returns bigint with 12 decimal representation (parseUnits(value, 12) / uint128) in result.value
    ✓ ignores errored sources (448 ms)
    ✓ counts errored sources in result.errors (683 ms)
    ✓ returns a source success report in result.sources (498 ms)
    ✓ extracts the median value for odd result lists (202 ms)
    ✓ extracts the the median value with average for even result lists (455 ms)
    ✓ returns all values for transparency in result.values (549 ms)
    fetchDataSource(config.source)
      ✓ throws if response can not be parsed as jon (19 ms)
      ✓ throws if the path is invalid
      ✓ throws if the value can not be parsed as number
      ✓ returns the number at the defined path in the fetched document (1 ms)
      ✓ supports http verb "GET"
      ✓ supports http verb "POST"
      ✓ supports sending a custom body
      ✓ supports sending custom headers
      ✓ supports hex values in response (1 ms)
      ✓ supports decimals values in response

Test Suites: 5 passed, 5 total
Tests:       35 passed, 35 total
Snapshots:   0 total
Time:        4.243 s
Ran all test suites.
```

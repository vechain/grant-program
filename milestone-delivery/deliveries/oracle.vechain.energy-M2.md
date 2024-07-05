
# Milestone Delivery :mailbox:

**The Ethereum address has been filled out correctly for this milestone, and the delivery is according to the official [milestone delivery guidelines](../).**

* **PR Link:** https://github.com/vechain/grant-program/pull/214
* **Milestone Number:** 2

## Milestone 2


| Number | Deliverable | Link | Notes |
|-|-|-|-|
| 2.1 | Configuration | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter
| 2.2 | Data-Loading | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter 
| 2.3 | Data-Extraction | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter
| 2.4 | Update-Check | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter
| 2.5 | Update Oracle | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter
| 2.6 | Feed Activity | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter

**The Reporter API documentation is also available:**

- https://node.vechain.energy/doc/swagger-ui/?url=https://raw.githubusercontent.com/vechain-energy/oracle.vechain.energy/main/reporter/public/swagger.yml#/


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

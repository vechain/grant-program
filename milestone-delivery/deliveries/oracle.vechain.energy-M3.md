
# Milestone Delivery :mailbox:

**The Ethereum address has been filled out correctly for this milestone, and the delivery is according to the official [milestone delivery guidelines](../).**

* **PR Link:** https://github.com/vechain/grant-program/pull/214
* **Milestone Number:** 3

## Milestone 3


| Number | Deliverable | Link | Notes |
|-|-|-|-|
| 3.1 | Value fetcher | https://github.com/vechain-energy/oracle.vechain.energy/tree/main/reporter/src/modules |
| 3.2 | Signer | https://github.com/vechain-energy/oracle.vechain.energy/blob/main/reporter/src/modules/signCcipRequest.ts |
| 3.3 | Deployment | https://oracle.vechain.energy/vet-usd |

**The Reporter API documentation is also available:**

- https://node.vechain.energy/doc/swagger-ui/?url=https://raw.githubusercontent.com/vechain-energy/oracle.vechain.energy/main/reporter/public/swagger.yml#/
- CCIP Requests can be tested manually `/{feedId}/resolver?sender={sender}&data={data}` endpoint in the swagger api


**Reporter Test Report**

```shell
$ yarn test --verbose
 PASS  src/modules/signCcipRequest.test.ts
  signCcipRequest({ request, config, report, env })
    ✓ signs the request correctly (36 ms)
    ✓ responds with (uint128 value, uint128 updatedAt, bytes32 feedId) (4 ms)
```

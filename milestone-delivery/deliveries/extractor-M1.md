# VeChain Ingestion Engine


* **PR Link:** https://github.com/vechain/grant-program/pull/191
* **Milestone Number:** 1

Integration with VeChain RPC, streaming data, parsing and decoding Transactions to be compatible with Extractor  feed. Integration with Kafka

Features are live in Production: https://extractor.live

The Product features announcement will be published on https://hacken.io/research/

### Milestone Details

#### M1: VeChain Ingestion Engine

| Number | Deliverable | Link | Notes |
| ------------- | ------------- | ------------- |------------- |
| 1. | Node RPC Interface | [trunk-vechain](https://github.com/syspulse/trunk3/tree/main/trunk-vechain) | mplementation of VeChain RPC spec interface to retrieve and parse data from node for the following entities: blocks, transactions, transfers, event logs. | 
| 2. | Ingest Streaming | [trunk-vechain](https://github.com/syspulse/trunk3/tree/main/trunk-vechain/src/main/scala/io/syspulse/haas/ingest/vechain/flow/rpc) | Ingest Streaming | Implementation of real-time streaming (Kafka Connect pipelines). | 
| 3. | Token Transfers | [ext-sentinel](https://github.com/haas-labs/ext-sentinel-workshop/tree/main/monitor) | Token Transfers are now implemented as part of Token Transfer Detector | 


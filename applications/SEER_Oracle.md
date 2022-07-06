# VeChain General Grant Application

## 1. Project Overview

- Project: SEER v1.0

- Team Name: Esol Labs

- Payment Address:

    - VeChain: 0xa2b13B6Be3fb3F9f98A43371687255D5943754Eb

    - Ethereum: 0xF4B57a2749Fa8FBFA9644a186e0730c2C64DcB90
    
    - Binance Smart Chain (preferred): 0xF4B57a2749Fa8FBFA9644a186e0730c2C64DcB90

### 1.1 Overview

**[SEER v1.0](https://oracle-stag.vebank.io/home)** is our first implementation of centralized, off-chain oracle infrastructure for applications built on VeChain. SEER provides real-time data feeds of 10+ key asset prices: BTC, ETH, VET, VTHO, VeUSD, and more, ensuring every dApps on VeChain networks can easily access reliable and trustworthy datasource.

Strategic values:

- Quick and easy to deploy.
- Easily accessible for dApp builders on VeChain.
- Price stabilization algorithm to protect from extreme price movements.

Our key emphasis is on stability and protection for users against extreme price movements and potential security risk. The use of reputable centralized exchanges ensure good pricing data input, and security risks are mitigated with price stabilization algorithms.

### 1.2 Project Details

#### _1.2.1 Introduction_

SEER v1.0 will have the following UI:
<img alt="Vebank" align="center" src="https://github.com/phamanhtai0410/test_readme/blob/main/static/assets/ETH.png?raw=true" width="100%" height="75%" >
<p></p>
<img alt="Vebank" align="center" src="https://github.com/phamanhtai0410/test_readme/blob/main/static/assets/BTC.png?raw=true" width="100%" height="75%" >
<p></p>
<img alt="Vebank" align="center" src="https://github.com/phamanhtai0410/test_readme/blob/main/static/assets/VTHO.png?raw=true" width="100%" height="75%" >
<p></p>
<img alt="Vebank" align="center" src="https://github.com/phamanhtai0410/test_readme/blob/main/static/assets/VEUSD.png?raw=true" width="100%" height="75%" >
<p></p>
<img alt="Vebank" align="center" src="https://github.com/phamanhtai0410/test_readme/blob/main/static/assets/SeerOracleDiagram.jpg?raw=true" width="100%" height="75%" >
<p></p>

#### 1.2.2 Calculate node logic

1. After getting data from Resource Pool, we will get a list of data about Multi-source Prices like this:

| **ID** | **Price** |
| --- | --- |
| DS1 | Value 1 |
| DS2 | Value 2 |
| DS3 | Value 3 |
| … | … |
| DSn | Value n |

Datasource will come from from exchanges:

| **ID** | **Datasource** |
| --- | --- |
| 1 | Binance |
| 2 | CoinBase |
| 3 | Kraken |
| 4 | Gemini |
| 5 | Poloniex |
| 6 | Kraken Crypto Watch |
| 7 | Vexchange |

2. Calculating Node will implement a function for choosing &quot;price&quot; at that moment: median, median\_low, median\_high,... This function is controlled by a Redis hash key stored in Redis Cluster. Now we got choosing\_price

    Ex: From 7 data sources, we get 7 prices of pair BTC-USD as below:

        [31021, 31018, 31001, 31009]

3. Algorithm: Using Exponential Moving Average (EMA) to calculate the price through time flow. Initial values:

    - Interval Period: SLIDING\_WINDOW\_INTERVAL = 5 (means each 5 seconds algorithm will be implemented one time)
    - Freshness Period: FRESHNESS\_PERIOD = 3600 (means each 1 hour, historic data used for the algorithm will be reset)
    - Flow chart:

    <!-- ![](</static/assets/CalculatingNodeDiagram.png>) -->
    <img alt="Vebank" align="center" src="https://github.com/phamanhtai0410/test_readme/blob/main/static/assets/CalculatingNodeDiagram.png?raw=true" width="100%" height="75%" >
<p></p>

For reference:

- Mockups: https://oracle-stag.vebank.io/home.

- Documentation of core components, protocols, architecture, etc. to be deployed: https://docs.vebank.io/welcome.

### 1.3 Ecosystem Fit

**VeThorChain (VeChain)** is a robust layer-1 blockchain with Proof-of-Authority consensus mechanism and is elected to the top 40 most popular global blockchain. The market capitalization of VeChain is recorded at over $2 billion dollars (at the time this application was first written), notably known for its duo-token system, VET and VTHO. With a mission to solve real-world problems on the blockchain, VeChain recently became the _UFC&#39;s first-ever Official Layer 1 Blockchain Partner_, actively promoting the development of DeFi infrastructure and adoption of its recent initiatives VeChain stablecoins (VeUSD) and Alchemy Pay. As total value locked (TVL) up to 10 million dollars is deemed to be an early stage of an ecosystem, VeChain became a fertile ground for developers to build large-scale DeFi projects. However, our study shows that DeFi protocols on VeChain are missing constant, seamless real-time external data feeds, which will eventually limit the ability to add more complex financial layers to the platforms, especially during the time crypto market faces high level of volatility.

In the future, our goal is to further enrich the ecosystem with more essential DeFi products, becoming the primary access point for data into the VeChain ecosystem. Further developments will involve:

(i) Decentralization: upgrade to a decentralized oracle.

(ii) More assets price data feed: support more assets for dApps on VeChain - we will be actively communicating with VeChain users to identify best fits to develop.

(iii) Expand to real-world data: one of our key goals is to get real-world use cases for blockchain dApps (ie. stock market, sport events, weather,... ).

## 2. Team

### 2.1 Team members
|||
| --- | --- |
| Team leaders: | Mr. Truong Phan (CEO) |
|| Mr. Tram Vo (CTO) |
| Team members: | Mr. Phat Nguyen (DevOps Team Lead) |
|| Mr. Hanh Nguyen (Frontend Team Lead)|
||+ 1 system engineer<br>+ 1 blockchain engineer<br>+ 1 backend engineer<br> + 1 designer<br>|

### 2.2 Team Website

#### 2.2.1 Team&#39;s experience

| Name | <p align="center">Experience<p> | <p align="center">Previous project/skill<p> |
| --- | --- | --- |
| Truong Phan | <ul><li>Senior Project Manager at Stably, Seattle-based stablecoin company.<li>6 years of experience leading product development for traditional finance and blockchain technology. | <ul><li>Stably various stablecoin projects: VeUSD on VeChain, USDS on Harmony, Chia, ICON,...<li> Gohub.vn - tech startup in e-SIM and telecom services |
| Tram Vo | <ul><li> Over 8-year experience in Software development<li> Deep experience in software development for large-scale systems, with over 25 million users and 2 million CCU at the 2018 AFC U-23 Championship.<li> Profound understanding of many subjects in software development such as requirement analysis, implementation, code review, testing, deployment process, alert and monitoring system.<li>Technical leader for 2 blockchain projects | <ul><li> Language: Python, Java, Solidity, Javascript, C/C++.<li> Database: MongoDB, MySQL, Redis, Firebase.<li> Tech: Docker, Redis, Micro-services architecture.<li> Cloud: GCP, AWS.<li> OS: Linux, Windows.<li> Blockchain: EVM, Truffle, Remix, Ganache.<li> Management: Agile, Jira. |
| Phat Nguyen | <ul><li> 7+ years of experience as a Senior DevOps Engineer with different server systems, especially streaming systems.<li> Experience in handling a large number of users (over 25 millions) | <ul><li> Media Streaming: Wowza, Nimble, Evostream, Nginx-rtmp.<li> Continuous Integration and Continuous Delivery: Jenkins, Ansible, Gitlab ci/cd.<li> Build Microservices architecture: Docker Swarm, Kubernetes.<li> Has experience with Cloud base systems (AWS / Azure / GCP).<li> Monitor system: Prometheus, netdata, zabbix, Grafana.<li> Log central: ELK, GrayLog.<li> Scripting languages: bash shell, python, Lua.<li> CDN: Nginx, Cloudflare.<li> Storage: Cephfs, Lizardfs, minio.<li> Mail server: Zimbra, ses aws. |
| Hanh Nguyen | <ul><li>Over 7 years in software development. | <ul><li> Database: MySQL, PostgreSQL, MongoDB.<li> Backend: PHP Node JS, Redis, rabbit MQTT , web service (RESTful APIs/SOAP).<li> Front end: Javascript/Typescript React , Web3, SASS/SCSS. |

#### 2.2.3 Team Code Repos

| **Platform** | **<p align="center">ID** |
| --- | --- |
| Github | https://github.com/seer-oracle |

#### 2.2.4 Team LinkedIn Profiles

| **Name** | **Linked in Profile** |
| --- | --- |
| Mr. Truong Phan | https://www.linkedin.com/in/buckphan/ |
| Mr. Tram Vo | https://www.linkedin.com/in/tram-vo-a72309199/ |
| Mr. Phat Nguyen | https://www.linkedin.com/in/phat-nguyen-kim-715481233/ |
| Mr. Hanh Nguyen | https://www.linkedin.com/in/hanh-nguyen-21839923a/ |

##


## 3 Development Roadmap

### 3.1 Example Roadmap for a dApp Application

- July 2022

    - Deploy SEER v1.0 oracle on VeChain testnet.
    - Supports price data feed for BTC, ETH, VET, VTHO, VeUSD.

- August - September 2022

    - Deploy SEER v1.0 oracle on VeChain mainnet.

### 3.2. Overview

|| Milestone 1 | Milestone 2 | Total |
| --- | --- | --- | --- |
| Estimated Duration | 2 month | 2 month | 4 months |
| Full-time equivalent (FTE) | 4 full-time engineers| 4 full-time engineers||
| Cost (up to $ 30,000) | Development cost: $10,000| Development cost: $10,000<br>Gas fee to keep the oracle running:$10,000 in $VTHO | $30,000 |

#### 3.2.1 Milestone 1 — Deploy SEER v1.0 on testnet
 
- Smart contracts for BTC, ETH, VET, VTHO, VeUSD data price on testnet.
- Website testnet on https://oracle-stag.vebank.io/home.
- Some smart contracts on testnet in currently:
    - SeerOracleVETUSD: `0x3212feD5581DEFbb2d7Ea21d7F22f657cD3da97E`
    - SeerOracleVETHOUSD: `0x5E7A52743575FE6F8cD8937C0415640338eBdd29`
    - SeerOracleVBUSD: `0xDf925feC9932A1De0d2b4404cCfac09166624F94`
    - SeerOracleVEUSDUSD: `0xA2B0d7b38dc13a58A7B4c0E8E2400d650dad46EC`
    - SeerOracleBTCUSD: `0x18A2fEAae2fA06B3452fd094Ba802C93FF0dA972`
    - SeerOracleETHUSD: `0xed8e829cfEB0Cdd315C26c7df10e81B12a3abA95`

#### 3.2.2 Milestone 2 — Deploy SEER v1.0 on mainnet

- Deploy smart contract for BTC, ETH, VET, VTHO, VeUSD data price on mainnet.
- Deploy official SEER website.

##


## 4. Future Plans

In the future, our goal is to further enrich the ecosystem with more essential DeFi products, becoming the primary access point for data into the VeChain ecosystem. Further developments will involve:

(i) Decentralization: upgrade to a decentralized oracle

(ii) More assets price data feed: support more assets for dApps on VeChain - we will be actively communicating with VeChain users to identify best fits to develop.

(iii) Expand to real-world data: one of our key goals is to get real-world use cases for blockchain dApps (ie. stock market, sport events, weather,... ).

## 5. Additional Information

What we have already accomplished:

- Smart contracts for BTC, ETH, VET, VTHO, VeUSD data price on testnet.
- Deploy beta website for SEER: [https://oracle-stag.vebank.io/home](https://oracle-stag.vebank.io/home).
- Run stress-test to test price feed stability with 100% accuracy and up-time.
- Ready for mainnet.

About other grants

- We haven&#39;t applied for any other grants.

Financial contributions

- Our team has self-financed this project from the beginning.
- Total budget that we have spent till date is about $20,000.
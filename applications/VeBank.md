# VeChain General Grant Application

**1. Project Overview** 

- Project: VeBank

- Team Name: ESOL Labs

- Payment Address:

-   VeChain: 0xa2b13B6Be3fb3F9f98A43371687255D5943754Eb

-   Ethereum: 0xF4B57a2749Fa8FBFA9644a186e0730c2C64DcB90

-   Binance Smart Chain (preferred): 0xF4B57a2749Fa8FBFA9644a186e0730c2C64DcB90

**1.1 Overview**

**VeBank** is a one-stop decentralized trading platform on the
VeThorChain (VeChain) blockchain. VeBank provides the major core finance
functions, but not limited to:

-   Trade: VeBank facilitates fast and cheap exchange of tokens with our automated market-maker (AMM)

-   Lend/Borrow: the non-custodial liquidity protocol on our platform
    allows users to participate instantly upon connecting to a wallet.
    As depositors, users can earn passive income by providing
    liquidity to the market. As borrowers, users can start borrowing
    in an over-collateralized (perpetually) or under-collateralized
    (one-block liquidity) fashion.

-   Farm: farming protocol allows users to deposit LP tokens and earn bonus rewards (not presented in this grant application)

-   Stake: users can stake $VB tokens to VeBank and earn platform rewards

VeBank protocol is implemented by a set of smart contracts on top of the
VeChain and is completely decentralized. No middlemen is involved so
users and applications can interact directly with the smart contracts,
the blockchain data, or via their favorite web3 providers.

**1.2 Project Details**

a.  How it works.

Demo video: https://www.youtube.com/watch?v=FhHClJG6aG8

*VeBank is an automated liquidity protocol powered by a constant product
formula and a system of non-upgradeable smart contracts on the VeChain
blockchain. It obviates the need for trusted intermediaries and
prioritizes decentralization, censorship resistance, and security.
VeBank is an open-source software licensed under the General Public
License.*

Each VeBank smart contract or pair manages a liquidity pool which is
made up of reserves of two VIP-180 tokens.

To enable trading on the decentralized exchange (DEX), there must be
liquidity. The liquidity provided to the exchange comes from Liquidity
Providers ("LP") who stake/deposit their tokens in the "Pools".
Anyone can become a LP by depositing an equivalent value of each
underlying token asset in return for the pool tokens. The tokens are
tracked pro-rata to the LP shares in the total reserves and can be
redeemed for the underlying assets at any time.



<img alt="Vebank" align="center" src="https://github.com/ttsang96/test/blob/main/media/image3.png?raw=true" width="100%" height="75%" >
<p></p>

Pairs act as automated market makers, standing ready to accept one token
for the other as long as the "constant product" formula is preserved.
This formula, most simply expressed as x * y = k, states that trades
must not change the product (k) of a pair's reserve balances (x and y).
Because k remains unchanged from the reference frame of a trade, it is
often referred to as the invariant. This formula has the desirable
property that larger trades (relative to reserves) execute at
exponentially worse rates than smaller ones.


<img alt="Vebank" align="center" src="https://github.com/ttsang96/test/blob/main/media/image4.png?raw=true"  width="100%" height="75%"  >
<p></p>


Because the relative price of the two-pair assets can only be changed
through trading, divergences between the VeBank price and external
prices create arbitrage opportunities. This mechanism ensures that
VeBank prices always trend toward the market-clearing price.


<img alt="Vebank" align="center" src="https://github.com/ttsang96/test/blob/main/media/image7.png?raw=true"   width="100%" height="75%" >
<p></p>


b.  How users interact with the protocol

The VeBank permissionless ecosystem is primarily composed of four types
of users: liquidity providers, borrowers, traders, and developers.

-   Liquidity providers (LP) are incentivized to contribute VIP-180
    tokens to common liquidity pools. The interest rates correspond to
    the earn rates, with the algorithm guaranteeing withdrawals at any
    time. In exchange, the LPs earn trading fees (LP tokens), which
    can also be staked to earn $VB tokens in the "farm". When a
    user makes a token swap (trade) on the exchange, he or she will
    have to pay a 0.3% trading fee, which is broken down as follows:


-   0.25% - Paid to liquidity pools in the form of a trading fee for liquidity providers (LP)

-   0.05% - Sent to $VB token farm

    <img alt="Vebank" align="center" src="https://github.com/ttsang96/test/blob/main/media/image2.png?raw=true"  width="100%" height="100%" >
    <p></p>


-   Borrowers are subject to risk evaluation of the asset loan,
    calculated Loan-To-Value, amount of funds available in the pool at
    time of borrow (the less funds incur the higher interest rates),
    and collateral policies. Liquidation modules would automatically
    trigger when predetermined liquidation thresholds are met. The
    table below shows a summary of the latest values:

  <img alt="Vebank" align="center"  src="https://github.com/ttsang96/test/blob/main/media/image1.png?raw=true"  width="100%" height="100%" >
  <p></p>


-   The protocol also incentivizes users to acquire liquidated assets at discount and with token incentives.

-   Traders can swap one token for one another at a fixed 0.30% fee which goes to liquidity providers at 0.25% and 0.05% to token farms.

-   Developers can interact with the open-source, accessible nature of VeBank. There are also many VeBank-specific tools built by the community.

Overall, interactions between these classes create a positive feedback
loop, fueling digital economies by defining a common language through
which tokens can be pooled, traded and used. VeBank's core lending and
borrowing will initially support VET, VeTHO, VeUSD and $VB and expand
to other big-cap assets in the future.


<img alt="Vebank" align="center" src="https://github.com/ttsang96/test/blob/main/media/image5.png?raw=true" width="100%" height="auto">
<p></p>


For reference:

- Beta site with full UI: https://beta.vebank.io

- Documentation: https://docs.vebank.io

**1.3 Ecosystem Fit**

**VeThorChain (VeChain)** is a robust layer-1 blockchain with
Proof-of-Authority consensus mechanism and is elected to the top 40 most
popular global blockchain. The market capitalization of VeChain is
recorded at over $2 billion dollars (at the time this application was
first written), notably known for its duo-token system, VET and VTHO.
With a mission to solve real-world problems on the blockchain, VeChain
recently became the *UFC's first-ever Official Layer 1 Blockchain
Partner*, actively promoting the development of DeFi infrastructure and
adoption of its recent initiatives VeChain stablecoins (VeUSD) and
Alchemy Pay. As total value locked (TVL) up to 10 million dollars is
deemed to be an early stage of an ecosystem, VeChain became a fertile
ground for developers to build large-scale DeFi projects.

VeBank aims to provide essential DeFi protocols on VeChain which improve
trading experience and increase total on-chain transaction numbers as
well as the total value locked. While it is obviously easy to clone EVM
lending dApps (like Aave, Compound) from Ethereum to VeChain, there is
not yet an Oracle available to support the core DeFi functions.
Therefore, we developed our own version of a centralized oracle (SEER),
and used it to provide multi-asset price feeds to VeBank.

VeBank Protocol is developed with security as our priority. An audit
third party will be involved to perform smart contract audits. Upon
completion, VeBank team will circulate the report to the VeChain
Foundation.

In the future, our goal is to enrich the ecosystem with additional DeFi
products, becoming the primary access point to the VeChain ecosystem.
The initiatives include cross-chain bridges to bring BTC, ETH and other
assets to VeChain, concentrated liquidity (similar to Uniswap v3),
stableswaps, NFT airdrops and NFT staking to boost lending/farming APY%.

## 2. Team

### 2.1 Team members
|||
| --- | --- |
| Team leaders | Mr. Truong Phan (CEO) |
|| Mr. Tram Vo (CTO) |
| Team members | Mr. Phat Nguyen (DevOps Team Lead) |
|| Mr. Hanh Nguyen (Frontend Team Lead)|
||+ 1 system engineer<br>+ 2 frontend engineers<br>+ 3 blockchain engineers<br>+ 3 backend engineers<br>+ 1 tester<br>+ 1 designer|

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
| Github | https://github.com/vebank |

#### 2.2.4 Team LinkedIn Profiles

| **Name** | **Linked in Profile** |
| --- | --- |
| Mr. Truong Phan | https://www.linkedin.com/in/buckphan/ |
| Mr. Tram Vo | https://www.linkedin.com/in/tram-vo-a72309199/ |
| Mr. Phat Nguyen | https://www.linkedin.com/in/phat-nguyen-kim-715481233/ |
| Mr. Hanh Nguyen | https://www.linkedin.com/in/hanh-nguyen-21839923a/ |

##

**3. Development Roadmap**

3.1 Roadmap


<img alt="Vebank" align="center" src="https://github.com/ttsang96/test/blob/main/media/image6.png?raw=true"  width="100%" height="75%" >

<p></p>

3.2. Overview

| | **Milestone 1** | **Milestone 2** | **Milestone 3** | **total** |
| ---| --- | --- | --- | --- |
| Estimated Duration | 4 months | 2 months | 2 months | 8 months |
| Full-time equivalent<br> (FTE) | 9 developers | 9 developers | 9 developers | |             
| Cost | $80,000 development<br> cost | $40,000 development<br> cost | $40,000 development cost<br> $30,000 audit fees | $190,000 |             

## 
<br>


*3.2.1 Milestone 1 --- Launch on VeChain testnet for the core lending functionalities* 

-   Complete research and development to arrive at MVP.

-   Complete design + UI mockup for the MVP website (https://beta.vebank.io) (beta.vebank.io)

-   Complete system infrastructure and user acceptance requirements for VeBank.

-   Complete development of following features: supply liquidity to
    lending pools, withdraw/repay liquidity from lending pools,
    liquidate a borrowing, claim incentive reward ($VB), claim
    incentive rewards, trigger safety/backstop module that liquidates
    up to 30% staked $VB for Short Fall event.

-   Determine risk parameters and collateral policies as well as platform fees.

-   Monitor lending pools with health factor <1.

*3.2.2 Milestone 2 --- Development & launch on testnet for trade, pool, and staking*

-   Enable Add/Remove liquidity pools, Stake/unstake $VB, and farming function.

-   Enable distribution of trading fees and protocol fees for users.

*3.2.3 Milestone 3 --- Official launch mainnet*

-   Perform smart contract audits with participation of a third party audit company.

-   Officially live on Mainnet for full functionalities of: trade, pool, lend & borrow, stake.

**4. Future Plans**

-   Develop VeBank NFT -> used to boost APY% for lend/borrow

-   Build a bridge system to allow seamless movements of big-cap assets from other blockchains to VeChain - BTC, ETH, BNB, etc to name a few.

-   Enable Futures/Options contract features on VeBank

-   Develop ETF-pegged assets (for example: stock index funds like VN30, VN-INDEX) to lend or borrow.

**5. Additional Information** 

Accomplished:

-   Deployed beta on beta.vebank.io (on VeChain testnet)

-   Deployed Lend/Borrow functions

-   Developed liquidation + safety module model.

-   Research and technical planning for DeFi Bridge, Vietnam ETF-pegged assets.

-   Whitepaper at docs.vebank.io

About other grants

-   We have not applied for any other grants.

Financial contributions

-   ESOL Labs team has self-financed this project from the beginning

-   Total expenses spent on this project are $50,000 which mostly cover technical development costs.


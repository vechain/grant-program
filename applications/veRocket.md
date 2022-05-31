# VeChain General Grant Application

## Project Overview 

- Project: VeRocket (formerly ZumoSwap)
- Team Name: VeRocket Team
- Payment Address:
- VeChain: `0xC6924234f79A86FfFE4F3129b052562188B71171`
- Ethereum: `0xa11d61e97dB398712c7Ef59f193DDC4d2Df9b0a9`

### Overview

**VeRocket** is a fast native decentralized exchange (DEX) running on VeChain. It provides a premium experience for users to swap tokens and earn by providing liquidity.

The reason to build a native DEX on VeChain is self-explanatory: providing a **low-fee environment** for users to exchange tokens. Thus enrich the use cases of VeChain and grow on-chain transactions. 

This incentive aligns with the vision of the VeChain foundation.

Thanks to the VeChain Foundation open-source initiative, we forked the UniSwap-v2 code and added our touch to the interface, which uses Sync2, Connex, Fee-Delegation, and MTT features.

### Project Details

We have already implemented a running version on VeChain: [Link](https://verocket.com). Here we list several features we have and will build into the project:

- Smart Contracts to support swaps and liquidity farming.
- It supports Sync, Sync2, and the VeChainThor wallet.
- A low fee of 0.3%.
- Multi-Task Transaction (MTT) feature to allow "one-click" swap.
- The exchange between any-to-any tokens.
- Improved automatic VTHO farming for VET assets.
- "Frictionless" swap using Fee-Delegation of VeChain (WIP)
- A chart to track DEX's status and user's holdings (WIP)

* Swap Interface
![P1. Swap](https://github.com/Tinto1024/grant-program-imgs/raw/master/imgs/1641460815959.jpg)
* Liquidity Interface
![P2. Liquidity](https://github.com/Tinto1024/grant-program-imgs/raw/master/imgs/1641460865938.jpg)
* Claim Interface
![P3. Claim](https://github.com/Tinto1024/grant-program-imgs/raw/master/imgs/1641460902636.jpg)
* Design of Fee Delegation Workflow
![P4. VIP-191 Architecture](https://github.com/Tinto1024/grant-program-imgs/raw/master/imgs/1641460466058.jpg)

### Ecosystem Fit
We see ourselves as a solid infrastructure of the VeChain blockchain system with only a 0.3% fee. 

By serving customers 24/7 and improving with new features from VeChain, we can improve the users' experience in swapping assets. 

Our daily transactions can also showcase the MTT and Fee-Delegated transactions. Improve total transaction volume on VeChain as a whole.

In the future, VeRocket will integrate with a bridge and lending service provided by other ecosystem parties and create a network effect.

## Team
### Team members
The team members require anonymity due to the regulations in their home countries, it is a high legal risk.

However, we understand the foundation wants to ensure the quialification of team members. The website https://verocket.com is our best demo of experience and you know best how huge improvement we have done based on foundation's open source code.

### Team Website

|    Platform    |                ID                   |
| -------------- | ----------------------------------- |
| Web            | https://verocket.com                |
| Twitter        | https://twitter.com/verocket        |
| Telegram       | https://t.me/verocket_official_chat |
| Business email | alex@verocket.com                   |

### Team Code Repos

| Platform |         ID                   |
| -------- | ---------------------------- |
| Github   | https://github.com/verocket/ |


### Team's experience
We have three years of coding skills in the blockchain domain (mainly on Ethereum).

After reading VeChain's open-source repo and documentation, we built our DEX interface with VeChain features (rather than forking Ethereum code) in the last two months.

The website https://verocket.com is our best demo of experience.

##  Development Roadmap
### Overview


**Total Funds: 22,000 USD**

|  Name   |    M1     |   M1.1    |    M1.2    |    M2     |            M2.1             |    M3     |
| ------- | --------- | --------- | ---------- | --------- | --------------------------- | --------- |
| Cost    | 3,000 USD | 1,200 USD | 12,000 USD | 1,200 USD | 100,000 VTHO (about 600USD) | 4,000 USD |
| Status  | Done      | Done      | Done       | Done      | Done                        | Done      |
| Man-Day | 12        |           |            | 5         |                             | 16        |

*Deliverables are too long to be described in the table so we describe them in the details below*

**We expect the foundation to exame our work and deliver the payments of M1, M1.1, and M1.2 at this time. Then after M2 is ready and online, deliver M2 and M2.1 upon contact.**

### Milestone Details

#### M1. Mutil-Pool, Multi-Tokens, MTT Feature in Query and Transaction.

At this stage, we built on top of VeChain Foundation open-source DEX code. We hired devs and designers, the work has been done is summarized as the following:
1) Add `any-to-any` token swap (route finding, rate calcuate).
2) Add `any-to-any` pool liquidity add/remove interface.
3) Implement the query of users' tokens balances and pool status to `multi-clause` calls.
4) Implement swap and liquidity-related actions to a `multi-clause` transaction.

#### M1.1 Launch: Server costs for 12 months
We hope the foundation can help us to cover the intial costs, but since 13th month we will earn money and sponsor ourselves.

We have rented servers and have run a VeChain node for data scraping:
1) Web server setup for swap service.
2) VeChain Thor Node server for data scraping.
3) Data analytics & storage backend server for charts.

#### M1.2 Audit: Report with a 3rd Party

This money doesn't pay to our team, but to audit firms.

We have negotiated with Certik, a minimum of 15,000 USD (5 working days) is required to cover the audit report.

HackenAI made an offer with even higher price (almost triple), which we think is too high and turned down the offer.

Currently our best offer is from Peckshield, with 12,000 USD.

Since VeRocket's smart contracts are nearly identical to foundation's open source code, 
**once audited, VeRocket will also donate the audit report with the VeChain foundation.**

Thus when other projects fork the code, they can also re-use this report.


#### M2. Fee-Delegation Feature

We implement a fee delegation feature to enable users to trade on VeRocket without paying VTHO fees.
1) Modify interface to allow VIP-191 workflows.
2) Establish a Node.js + MySQL server to sign transactions.


#### M2.1 Fee delegation VTHO sponsor (For VeUSD event)

100,000 VTHO is about the cost of 25,000 swaps.

At this stage, we will contact the foundation to sponsor VTHO to cover our bootstrap trading competition for the VeUSD launching event.

The money will be solely used for paying users' transactions to boost on-chain transactions.

#### M3. Charts

Similar to [Uniswap Chart](https://info.uniswap.org/#/), **Chart** is a key part of the DEX info.

This requires a database, a set of APIs and a web page to display. 

We expect this to be a **full-time-equivalent engineer and a designer working for two weeks**.

The **working result** will be a web page on `charts.verocket.com` and a set of **open-source Javascript or Python SDKs** for scraping data. This can largely benefit the VeChain Community.


### Community engagement

We tackle the users on the social media platforms described in above sections.

On Medium we plan to release monthly reports, on Twitter every second day, and we have a Github for documentations.

We are a active project on Twitter, **22 tweets** have been published so far. And some tweets have been retweeted by the foundation and CREAMethod.

The continue of exposure of Telegram, Twitter and Medium is expected from us. We post tweets constantly about tech updates and fixes bugs reported by users, since launch we have fixed 16 bugs mentioned.

We will also initiate airdrops events for early adopters soon. VeRocket is at early stage, it will continue to evolve to be the best DEX on VeChain.

## Future Plans
Plans are straightforward:
- Maintain the DEX and make money to support ourselves.
- Integrate with CoinMarketCap (CMC), business talk on-going.
- Integrate with VeStats and provide tech support and insight, business talk on-going.
- Integrate with tokens and bring more tokens to the eco-system, like VeUSD. Business talk on-going.
- Establish a token incentive scheme to ensure the longevity of the DEX (no token sale, pure community style).
- Develop a 2nd generation of DEX.
- Explore **lending protocols** and push VeRocket to a multi-chain environment.
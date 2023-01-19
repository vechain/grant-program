# VeChain-CryptoSlam
Project: Integrate VeChain blockchain on CryptoSlam platform

Payment Address: 0x5aE970dcb37067Aed6F9578b64482dF9D91622B3


# Overview
- CryptoSlam is a data aggregator tool for the NFTs that connect Collectibles, Art and Game communities enables NFT data for over 20 high-volume blockchain:
    - Ethereum
    - Solana
    - Cardano
    - Flow
    - Polygon
    - BNB
    - ImmutableX
    - Panini
    - WAX
    - Tezos
    - Avalanche
    - Ronin
    - Arbitrum
    - Algorand
    - Palm
    - Cronos
    - Fantom
    - Waves
    - OEC
    - Zilliqa

We continue growing our user base and onboarded chains month over month. 

Our core strengths are custom calculations, onboarding speed and data evaluation process. For all onboarded chains we cover 100% of the collectiolns and constantly enable APIs to support the onboarding of the new projects. 

CryptoSlam offers accurate NFT numbers, community and data maintnance to make Vechain get more traction, acquire new projects and build a stronger community.

# Project Details 
- Onboarding
    - Connect with all Ve chain Marketplaces
        - World of V
        - VeSea
        - VPunks
        - VimWorld
        - NFR Paper Project
        - BlackVeMarket
    - Backfill all collections on CS
    
    ![Screen Shot 2022-12-06 at 1 13 40 PM](https://user-images.githubusercontent.com/121036746/208442943-15b2c530-fc2c-4d66-b031-e1213bd4302f.png)

- VeChain explorer
    - Sales Volume
    - Collection Rankings
    - Data Viz - Charts
    - Top Sales
    
    ![Screen Shot 2022-12-06 at 1 14 58 PM](https://user-images.githubusercontent.com/121036746/208443477-6345461f-7e64-451d-a042-f2aca9bcd578.png)


# Technical Roadmap for Onboarding VeChain

NFT tracking will be implemented by reading clauses in every transaction for each block and decoding the inputs and events of the clauses.

We start with the transfer events including mints. Then we move to the sales which are usually not standardized, so we would have to parse the events and find all the transfers of the NFTs and corresponding payments that happened within the same clause. Last piece is getting the metadata for NFTs by using their tokenURI.

As soon as everything is implemented for tracking we are making a test period of live tracking to verify the accuracy, fixing the bugs if any and enabling historical crawl of the blockchain to have all the NFTs being tracked and setup on the platform.

To have the required accuracy and reliability we will have to setup a node/api or find a source to use.

## Overview
|  | Milestone #1 | Milestone #2 | Total |
| --- | --- | --- | --- |
| Estimated duration | 2.5 months  | 1 week | 3 months |
| Full-time equivalent (FTE) | 1 | 1 |  |
| Cost  | $28,000 | $2,000 | $30, 000 |

## Milestone #1
| Number | Deliverable | Specifications |
| --- | --- | --- |
| 1 | Investigate nodes | Investigate and setup best way for getting data out of a blockchain, check external providers |
| 1.1 | Organize transaction types/events from the blockchain | Identify possible transaction types, events, structures, setup tracking and storing of those transactions |
| 1.2 | Get tokens metadata | Get all NFTs metadata from blockchain |
| 1.3 | Onboarding | Setup automation to pick up any new collections being created on the blockchain |

## Milestone #2
| Number | Deliverable | Specifications |
| --- | --- | --- |
| 1 | Sales summary  | Include all historical data and data visualization  |
| 1.1 | NFT Collections | All VeChain collections with the rankings  (Sales, transaction,  Seller/Buyer wallets, Owners count) |
| 1.2 | Top Sales | Price (Crypto, USD), Seller/Buyer wallets |

## Team
| Team | Contact Person|
| --- | --- |
| Engineering Lead  | Artem Kharlov |
| Marketing | Yohann Calpu |
| Community  | Yehudah Petscher |
| Product | Pasquin Rahming |


    

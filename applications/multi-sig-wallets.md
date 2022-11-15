# VeChain General Grant Application Template

## Project Overview 

- Project: Multi-Signature-Contract and Administration
- Team Name: favo
- Payment Address: `0xcC4B3412161Ea88d0538D2Da15cffa74af0eE9D4`

### Overview

At the moment there exists no publicly available solution for shared responsibility of a wallet. With the growing size of projects it becomes more and more important to share access to single wallets between multiple parties instead of relying on trust of a single one.

Ethereum solves this with smart contracts and apps managing them.

This project aims to migrate an existing solution from Ethereum to VeChain. Everything will be created Open Source to verify and with the ability run locally. The Administration will be channeled into Sync2.

### Project Details

#### Smart-Contract

Gnosis.io is one of the best known solutions on Ethereum. Gnosis also has GitHub repositories open sourcing its solution.

The first goal is to adjust and ensure it deploys on VeChain correctly with the following goals:

1. Avoid adjusting the contracts code
1. Favor a deployment only project over a cloned modified project (to ensure responsibility stays within Gnosis)
1. Provide instructions on how to deploy on VeChain

#### Management-Application

The management of the Multi-Sig-Wallet will be built into Sync2 as a new Wallet-Type.
This ensures the users experience is ecosystem consistent and builds on top of the existing wallet solution.

- During wallet creation the user can select to create or import a new Multi-Sig-Wallet. The creation deploys a new contract on the network.
- On the address cards information about pending transactions are shown.
- When interacting with VET or Tokens, the Multi-Sig-Contract is used. The interface is adjusted accordingliy.
- Goal is to implement the Wallet-Handling as smooth as possible into the current flow.
- The modified Sync2-Wallet will be available for everyone to download and build locally and as a deployed web-application.


### Ecosystem Fit

It is an important security functionality that is widely used but currently missing in the ecosystem. It will increase security for bigger projects and wallets.

## Team 

### Team members

- I am a fulltime IT-professional for 24 years with focus web- and mobile applications. I am happy to share more details by email (instead of publishing it on GitHub).

### Team Website

- https://vechain.energy


### Team's experience

* 24 Years of development experience, team management and company management
* Heavily driven by Test-Driven-Development

## Development Roadmap 

#### Overview

|  | Contract | Backend | Total |
| - | -: | -: | -: |
| Estimated Duration | 8d | 20d | 28d |
| Full-time equivalent (FTE) | 1 | 1 | 1 |
| Cost (up to $ 30,000) | $6,400 | $16,000 | $22,400 |

Development costs are based on a daily rate of $800 per developer for a regular work day.


#### Milestone 1 — Contract

| Number | Deliverable | Specification |
|-|-|-|
| 1.0 | Instructions | A Markdown manual in a git repository explaining on how to setup a Multi-Sig-Contract |
| 1.1 | Deployment-Scripts | All required scripts and processes to deploy a new Multi-Sig-Contract on the Test and MainNet using the command line |

* Delivery will be by a public repository with the complete source code
* A sample web application is be published to test basic functionality:
   1. deploy a new contract
   2. basic interaction of
      1. adding a new owner
      1. removing an exiting owner
      1. creating a request to send VET
      1. creating a request to send a VIP-180 Token
      1. authorizing a payment
      1. rejecting a payment

#### Milestone 2 — Sync2

| Number | Deliverable | Specification |
|-|-|-|
| 2.0 | Multi-Sig-Deployment | Ability to deploy a new Multi-Sig-Contract during Wallet-Creation |
| 2.1 | Multi-Sig-Deployment-Configuration | Configuration option (in Code) to disable Multi-Sig-Contract deployment to remove potential responsibility from the Wallet |
| 2.2 | Multi-Sig-Import | Ability to import an existing Multi-Sig-Contract during Wallet-Creation |
| 2.3 | Multi-Sig-Wallet | Overview of the balance of a Multi-Sig-Wallet and relevant meta information |
| 2.4 | Create Transaction | VET and Tokens create a transfer request  |
| 2.5 | Transaction Management | List of pending requests with the ability to approve and reject transations|
| 2.6 | Owner-Management | List of owners and the ability to add a new or remove an existing owner |
| 2.7 | Web-Deployment | Deploy the web-version on a custom website |
| 2.8 | Pull-Request to Sync2 | A documented Pull-Request is provided to the official Wallet |

The modification will be made to Sync2.

1. Delivery will be by a publicly forked repository with the complete source code
1. The web-version of Sync2 will be published on a custom URL for delivery.
   1. If the Wallet-Maintainer decides to accept the merge request, it will be part of the official Sync2 wallet.
   1. A configuration option to disable Multi-Sig-Contract-Deployment in the official Wallet is given to remove potential responsibility from the Wallet.
   1. The custom deployment of the web-version allows to deploy the contract.


#### Community engagement

At least one medium article and tweet will be published on how to setup a Multi-Sig-Wallet. Additional support will be provided in Discord or via issues.

## Future Plans

A on-going-maintenance of the project is planned as a personal investment and the Open Source character allows the community to participate and maintain as well.  
On top a Multi-Sig-Contract-Manamgement-Platform is planned for vechain.energy that is not scope of this grant.

## Additional Information 

Reserch and basic testing for an MVP was already done. I have received a grant for the basic development of vechain.energy.

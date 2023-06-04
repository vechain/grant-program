# VeChain Mobile V3-Swap Grant Application

## Project Overview 

- Project: A mobile V3-Swap 
- Team Name: SayNode Operations AG 
- Payment Address: 0x989A38EDEbd2Bd80d4949a9F7462C93FA8055876


### Overview

With the V3-Version of Uniswap the company brought major changes to how v2 worked. V3 introduced the concentrated liquidity which represented a significant advance since it gives liquidity providers control over the price range wherein their assets were transacted. In addition it allows users to choose from different tier levels (0.05, 0.30, and 1%). As of now there is no DEX on VeChain that offers these functionalities.

The project is to create such a DEX with these mechanics. But instead of just creating a regular website, as everyone has done so far, we are creating a mobile application for Android, with the possibility of extending it to the iOS store if possible. Such an App would be the first of its kind. 


# Tools and Features
  - It will connect to the Sync2 wallet
  - Pools with Vechain will obviously produce VTHO. The creator of the pool can chose if he wants that VTHO to pay for the pool users swaps using the Designated Fee Delegation;
  - Users can make multiple swaps in one go making use of the multi clause transactions;

### Project Details

- Mockups/designs of any UI components
  Launch Screen | Wallet Screen
  :-------------------------:|:-------------------------:
  ![](https://drive.google.com/uc?id=1In0rO4y02hIFSpagPtIgmtIpE-8pu7XP) | ![](https://drive.google.com/uc?id=1i-ntWtaKPFlJWa756uCUwCGO7gvr0aIo)

  | Set Position Screen |     Swap Screen     |
  | :-----------------: | :-----------------: |
  | ![](https://drive.google.com/uc?id=1TgqVAqWALv39aC61NFWH9UVIzIvcihdB) | ![](https://drive.google.com/uc?id=1dcRSqWu1B-0M_532g_0Dc6YbYqLdmb_W) |

- An overview of the technology stack to be used

  The smart contracts will be fully written in Solidity.
  The testing of the smart contracts will be done in Python, first with Brownie in a locally run copy of Ethereum, and finally in real time with the Vechain testnet.
  The frontend will be written in Flutter making use of the [thor-requests Dart library](https://pub.dev/packages/thor_devkit_dart), previously designed by our team.

- Documentation of core components, protocols, architecture, etc. to be deployed
  The project will be divided into 2 main contracts:

  1. The pool smart contract: implements the swaps, the position setting and the position modification;
  2. The pool deployer contract: deploys and keeps track of the deployed pools;

  It will also make use of several library contracts to aid in the complicated calculations (fixed point math, bitmath, tick to price and price to tick calculations, token amount calculations, liquidity calculation, etc).

  The general workflow/architecture is as follows:

  1. Users can create new pools by specifying the two token addresses and the fee amount they wish to charge per swap;
  2. The pool id is created based on the fee and the two token addresses, and stored in the factory contract. We can invoke pools by calling the factory contract with the corresponding fee and addresses of the pool we want to use;
  3. The created pools can be initialized by specifying its initial price;
  4. Users can set ranged positions, preform swaps, check and alter their positions.

  ![alt text](https://drive.google.com/uc?id=1PRImlILOoerezAf56Veu7vETbNDKIZAD)

  Because the AMM is segmented (aka has different liquidities in different price ranges), the token amounts when setting a position are different depending on where the price range is compared to the current pool price. \
  The swap calculations also require attention, but are overall simpler.
  All of these different situations will be included in the contracts and all the calculations are made inside the contracts, to avoid mathematical rounding errors between the frontend and smart contract languages.

  The UI will allow the user to easily create or pick existing pools to swap or set a position in. The users will also be able to see all of their current positions (pool it is in, price range, liquidity and fees gained) and edit them.

- PoC/MVP or other relevant prior work or research on the topic

  To prepare for this project, the authors researched several sources, listed bellow:

  - https://uniswap.org/whitepaper-v3.pdf
  - https://atiselsts.github.io/pdfs/uniswap-v3-liquidity-math.pdf
  - Source code study in: https://github.com/Uniswap/v3-core and https://github.com/Uniswap/v3-periphery
  - Code was forked, tested and changed for further understanding

### Ecosystem Fit

- Uniswap is one if not the most used DEX as of today. One of the reasons why are some of its unique functionalities. For VeChain creating such a swap would be an extension of the existing Ecosystem and offering users something new. Furthermore, by creating an App for Android with the option of extending it to the iOS-Store the VeChain ecosystem offers a flawless and unique user experience.

## Team 

### Team members

The company has about 20 employees. The most relevant persons (e.g. team leaders) for the implementation of the project are mentioned below. 

- Renato Schär
- Werner Liechti
- Yann Marti
- Paula Amstutz
- João Morais
- Rodrigo Dias


### Team Website

- https://saynode.ch/

### Team's experience

- SayNode stands out for having the tech stack that combines blockchain and mobile development. We strongly believe that perfect user experience will be the key for a successful Web3 project. 
The team around SayNode has already implemented various projects in the Web3 area. For this grant application the most important are the experiences, which were collected with the project https://raclette.finance/. Thereby the logic of Uniswap V3 was provided for the Tezos-Chain.  Besides that, a grant for the Dev-Thorkit-Dart has already been granted and this project will include the same developers. Also, SayNode already deployed two Flutter Apps, which have been accepted in both Apple Store and Android Store. Overall, the team has experience with DAO creation, wallet creation, tokens and multichain tokens, ICOs and everything around App-Development.


### Team Code Repos

In addition to the project and team repos mentioned below, we would also like to focus on https://raclette.finance/ which was created by our team. For confidentiality agreements no repo can be released for this project yet. As soon as the audit is complete, this will be made public. 

- https://github.com/SayNode/thor-devkit.dart
- https://github.com/SayNode/thor-request.dart
- https://github.com/SayNode/DAO-VeChain
- https://github.com/SayNode/axper
- https://github.com/SayNode/supply_chain_resilience_final
- https://github.com/SayNode/Vidaia
- https://github.com/RsTs23
- https://github.com/wernerliechti
- https://github.com/YannMarti
- https://github.com/paulamstutz
- https://github.com/Krfld

### Team LinkedIn Profiles

- https://www.linkedin.com/in/renato-sch%C3%A4r-8a9a19a5/
- https://www.linkedin.com/in/werner-liechti-568b19213/
- https://www.linkedin.com/in/paula-amstutz/
- https://www.linkedin.com/in/joaogmorais/
- https://www.linkedin.com/in/simon-heer-202866110/
- https://www.linkedin.com/in/krfld/

## Development Roadmap

#### Overview

|                            | Milestone 1 | Milestone 2 | Total |
| -------------------------- | ----------- | ----------- | ----- |
| Estimated Duration         | 60 d        | 30 d        | 60 d  |
| Full-time equivalent (FTE) | 1.5         | 1.5         | 10    |
| Cost (up to $ 30,000)      | 20000       | 10000       | 30000   |

#### Milestone 1 — Smart Contract development and test

| Number                                                                                               | Deliverable                                   | Specification                                                                                                                                                                                                                     |
| ---------------------------------------------------------------------------------------------------- | --------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0a.                                                                                                  | Documentation                                 | We will provide simple documentation for each contract, explaining their main functions nad their roles.                                                                                                                          |
| 0b.                                                                                                  | Testing Guide                                 | The code will have proper unit-test coverage (e.g. 90%) to ensure functionality and robustness. We will describe how to run both the Brownie and Vechain testnet tests.                                                           |
| 1a.                                                                                                  | Smart Contracts: Development                  | We will develop smart contracts that will deal with pool creating and indexing (Pool Factory contract) and with the pool operations (swaps, position setting, checking and changing).                                              We will open source the smart contracts and upload the ABI to [B32](https://github.com/vechain/b32). |
| 1b.                                                                                                  | Smart Contracts: Testing with Brownie         | We will create several tests in Brownie. Because brownie allows us to run a mock up of the Ethereum blockchain and simulate the passage of time, we can run several tests in a matter of seconds, making it easier for debugging. |
| 1c.                                                                                                  | Smart Contracts: Testing with Vechain Testnet | We will replicate all the Brownie tests but with regular Python scripts, using the thor-requests library and the testnet. This way we can make sure there is no functionality loss between blockchains.                           |

#### Milestone 2 — Frontend

| Number | Deliverable           | Specification                                                                                                                                                             |
| ------ | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1      | Frontend: Design      | We will create the UI design in order to make it appealing and intuitive. Colors schemes, button formatting, location of elements, etc, will all be done i this phase.    |
| 2.a    | Frontend: Development | The previously planned UI will be build and organized.                                                                                                                    |
| 2b.    | Frontend: Integration | The frontend will connect to the contract                                                                                                                                 |
| 2c.    | Frontend: Testing     | Several tests will be run to make sure everything works correctly: the UI works as intended and page load up speed/performance. The contract interaction is also checked. |
| 2d.   | Frontend: Tutorial | Simple guide on how to swap and set, check and change positions. |
...

#### Community engagement

Currently, SayNode is in the process of building a marketing team. For this purpose, at least one new full-time position will be created which will take over all marketing activities. Thus, we can play on different channels simultaneously and professionally. In addition, SayNode holds a Meetup once a month in Switzerland, where the product is promoted. This effort will be further expanded, so the goal is to hold at least two events per month starting in May. This also includes a webinar to create geographical independence. At all events the product will be promoted directly. 

In addition, the known channels such as Medium and blogs will be used directly. 


## Future Plans

SayNode future plans with the project are to actively maintenance the app, to market it and to build a loyal customer base. In a second step, as soon as Apple allows it, the app will be adapted to meet Apples regulatory standards. 

## Additional Information 

- What work has been done so far?

For the UI we have already created first mockups (visual). And we have established the know-how from our Tezos-Project.

- Are there any teams who have already contributed (financially) to the project?

--> no

- Have you applied for other grants so far?

Yes, we have requested VeChain grants in the past, but not for this project. 

# VeChain General Grant Application Template

## Project Overview

- Project: Vechain integration in Cosmoly
- Team Name: CosmolyLabs
- Payment Address: 0xD81F2144996A9A1eB0d9B8260bab25f5485466f0

### Overview

Please provide the following:

- Cosmoly is a app that allows users to interconnect wallets from different blockchains through a single platform. A place where you can exchange, send, receive and save between multiple chains using a single platform with just your wallet.
- Vechain is a fairly fast and low-cost protocol, but its DeFi ecosystem still needs to be more robust. We want to implement it on the platform so that users can access more tokens and different blockchains, natively using only their wallet.
- Not only is it another app on vechain, it would bring the use of more tokens, active users and new savings systems (or staking) which would be a perfect opportunity to create new opportunities for developers

### Project Details

Cosmoly is a set of decentralized protocols and services, which operate across different blockchains. Although it can be divided into the following core services:

#### External services

- **Li.Fi Integration:** Providing Liquidity from 28+ DEXs and 15+ Bridges and +22 different blockchains
- **Onramper:** Providing 17 onramps and 182 local payment methods.
- **Nexo Earn API**: Off-chain earning services with 5-16% APY (only with some tokens and stable coins)

#### Internal services

- **Bridge between VeChain and Polygon (and 22 blockchains more):** This would allow VeChain to connect (using polygon) to the more than 22 different blockchains of the Li.Fi protocol. Without the need to go through an CEX, registrations or verifications.
- **Earn protocolo in VeChain:** Earn daily interest using VeUSD, VET and Cosmo-USD (a token collateralized in USDC/USDT).
- **Creation of COSMO-USD:** A token collateralized in USDC/USDT on the polygon blockchain, which, using the Li.Fi protocol, connects to more stablecoins.

#### Benefits of working with VeChain Services

- Great overall support from the Vechain team
- Increase in user adoption for Vechain tokens and DeFi ecosystem
- Lower Gas fee
- Faster transaction confirmation times

#### Documentation

You can check our Litepaper at: <https://docs.cosmolylabs.com>

#### MVP

We are a team focused more on action, you can check our platform at <https://cosmolylabs.com>

### Ecosystem Fit

Here is our competitive advantage, there is no project of this category on VeChain. The only closest competitors would be the CEX, which are in another market category.

And according to <https://apps.vechain.org/#defi> the only application with a bridge function is <https://swap.vechain.energy/> but it does not have savings functions

Our idea is to connect Vechain's currently operating DEXs, to increase liquidity, obtain the best rates and improve the user experience

## Team

### Team members

- David Gimenez (Full Stack Developer | Blockchain Developer | Graphic Designer UI/UX | CEO CosmolyLabs)

### Team Website

- <https://cosmolylabs.com>

### Team's experience

I am David Gimenez, an experienced software developer and entrepreneur with a special focus on blockchain, finance and UI/UX design. I have a strong background in TypeScript, React.js, Angular.js, Flutter, Python, MongoDB, SQL, Solidity, Web3 and PyTeal.

I have a passion for creating efficient, high-quality and user-friendly applications which are both secure and reliable. I strive to stay up to date with the latest technologies and industry trends by attending conferences, workshops and online courses.

Throughout my career, I have worked on a wide variety of projects, from complex multi-node architectures to user experience design. I have a strong eye for detail, and I am always ready to take on challenges.

You can check my LinkedIn to know more about me.

For smaller tasks (marketing, smart contract audits, graphic design, UX/UI creation for Vechain integration) external agents would be hired (using Fiverr or Upwork)

### Team Code Repos

- <https://github.com/AgentDavid>

### Team LinkedIn Profiles

- <https://www.linkedin.com/in/davidgx100/>

## Development Roadmap

|  | Milestone 1 | Milestone 2 | Total |
| - | - | - | - |
| Estimated Duration | 60 d | 30 d | 90 d |
| Full-time equivalent (FTE) | 3 | 2 | 5 |
| Cost (up to $ 30,000) | $ 15,000 | $ 10,000 | $ 25,000 |

### Milestone 1 — Smart Contract & Backend

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | Apache 2.0 / MIT / Unlicense |
| 0b. | Documentation and System Architecture | We will provide inline documentation of the code, a detailed system architecture description, and a basic tutorial that can interact with the deployed smart contracts and backend service. |
| 0c. | Testing Guide | The code will have proper unit-test coverage (e.g. 90%) to ensure functionality and robustness. In the guide, we will describe how to run these tests
| 1 | Smart Contracts | We will develop smart contracts that will allow the exchange (mint and burn) of tokens collateralized in Polygon using VeChain. Where you can create new tokens (mint) and redeem tokens (burn). The token to be developed will be COSMO-USD. A functionality will also be created to earn in COSMO-USD natively in Vechain .  We will open source the smart contract and upload the ABI to [B32](https://github.com/vechain/b32). |
| 2 | Backend | We will create a backend service that once the swap from COSMO-USD to USDC/USDT is made (in Polygon).  The user can choose another destination token using the Li.Fi protocol. In addition to managing the smart contract of the earn module in COSMO-USD of VeChain|

### Milestone 2  —  Frontend

| Number | Deliverable | Specification |
|-|-|-|
| 1 | User Guide | We will provide a user guide or a demo video to show what features have been done.  |
| 2 | Page Implementation | A page will be added exclusively for vechain users on the cosmoly platform, where they can manage COSMO-USD, earn, exchange, redeem or send. In addition to providing an attractive and simplified user experience  |
| 3 | Onramper Implementation | A page is added so that users can purchase USDC (or any other token) using their local currency. So that they can later exchange it for VET, or use Vechain for the first time  |

## Community engagement

Telegram: <https://t.me/CosmolyLabs>
Twitter: <https://twitter.com/cosmoly>
Instagram: <https://instagram.com/cosmoly.labs>

## Future Plans

More VeChain DEXs are planned to be connected to the cosmoly platform, so the user can compare the best options when making exchanges.

## Additional Information

- An [NFT](https://rarible.com/token/polygon/0xb14b13441950bf9cf88ebd2d32c92b369dd79556:97754577160056121414870082490933494409269140691460412199306832292365318750209) was created in polygon that represents 20% of the participation in the cosmoly project
- AI-based trading functions are currently planned to be implemented
- It has been applied to external grants but they do not include the implementation of VeChain in the project

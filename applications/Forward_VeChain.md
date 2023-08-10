# VeChain General Grant Application Template

## Project Overview

- Project: Forward Protocol
- Team Name: Forward 
- Payment Address: 0x182CebAB47af1302F39A3dE67dA8BA3945341690

### Overview
*---A brief description of the project---*

Forward Protocol is WordPress of Web3.0. Users with zero technical knowledge can build and deploy full-stack dApps, subnets and even blockchains in very little time and minimum cost involved with an easy-to-use, drag-and-drop no-code interface. These dApps (full-stack applications) can be deployed directly to VeChain or any EVM and Rust compatible chain.

Forward also has an Open Marketplace where developers can upload and build their own template dApps for which they can set a fee or monetization structure for the usage of their templates.

Languages which we support are Solidity, with Rust and Move coming soon. Python and Go are also on our roadmap.

*---An indication of why your team is interested in creating this project within the VeChain Ecosystem---*

Due to VeChainThor being EVM compatible, Forward can integrate VeChain with the Forward platform to allow any Forward user to directly build and deploy dApps to VeChain easily.  The VeChain wallet will also be integrated. By doing these integrations, the deployment of dApps and users on VeChain are increased.

*---If relevant, an indication of how you will integrate tools and features (e.g., Sync2/Connex, fee delegation protocols, MTT, etc) to enhance your project---*

Stepping into the future of Web 3.0, our project aims to accommodate all the features of a WordPress like environment for the VeChain Ecosystem. Catering to users with diverse skills, it simplifies the creation and deployment of full-fledged dApps, subnets, and even blockchains. This is achieved through an intuitive, drag-and-drop, no-code interface that requires minimal time and cost.

Our project goes the extra mile to ensure a user-friendly environment. By integrating powerful VeChain tools such as Sync2/Connex, we bridge the gap between dApps and the VeChainThor blockchain. Similarly, we can look at ways VeChain's fee delegation protocols are harnessed to delegate transaction fees to our sub networks, sparing users from the need to hold or spend VET or VTHO tokens but still able to utilize the VeChain network. Additionally, the multi-task transactions feature enables users to carry out several actions within a single confirmation, promoting efficiency. If needed, this feature can potentially enable users to set up network nodes, contracts, and a dApp all in a single interaction, again all while eliminating the need for coding.

However, this powerful suite doesn't come without its challenges. Adopting VeChain's unique ecosystem may pose a learning curve to our developers. Given the prominence of Ethereum and other blockchains, users may not immediately see the value in VeChain features. Moreover, security and maintenance considerations require vigilant oversight.
Nevertheless, our project stands as a promising platform for users interested in VeChain, offering a unique blend of efficiency and user-friendliness. We're committed to providing an environment that supports the evolving needs of our users, bolstered by the robust functionalities of the VeChainThor blockchain.

To top it all off, our project boasts an Open Marketplace. Here, developers can upload and monetize their own template dApps, further enriching the platform's offerings. Currently, we're fluent in Solidity, with Rust and Move on the horizon. The roadmap also includes plans for Python and Go ensuring a diverse and robust development landscape.

![Forward Protocol Overview](https://drive.google.com/file/d/1TLY4eZp5G8q4vEowq_arVoRDnhunjSn8/view?usp=sharing)

### Project Details

**More detailed info can be provided in private as the info is of a proprietary nature**

*---Mockups/designs of any UI components---*

![Getting Started](https://drive.google.com/file/d/15lBmb6SQIEe3IQNjRymP66_U46dTjjO8/view?usp=sharing)

![Forward Factory](https://drive.google.com/file/d/1M52zQM68mFg9oRYQBwtlpK8hdFRSpQgR/view?usp=share_link)

![Forward Marketplace](https://drive.google.com/file/d/1na94BkJ_sz4-Q8-QoXEvWwkCfUwCthoc/view?usp=share_link)

![Forward Drag-and-Drop Builder](https://drive.google.com/file/d/108XSVRtR0Y0al_bGxqmOBcX2jz5PsXPz/view?usp=share_link)

![Forward Purchase and Deploy](https://drive.google.com/file/d/1xnwnyLN43LoEHdJ356wLoAb0gVwA_Xw6/view?usp=share_link)

*---API specifications of the core functionality---*

Forward’s API interface allows our developers to utilize and create white-labeled websites or drop-shipped applications.

This allows for medium or larger enterprises to set up their own custom portals utilizing our software and connecting to our functions/network.

This means that it will make it much simpler for enterprises or businesses to access the SDKs for multiple blockchain networks but still hold onto their own marketing/identities. It also enables them to restrict their contracts to their potentially upscaled clients.

![Forward Network Overview](https://drive.google.com/file/d/1qWDZNW6Rl-EsebXUy4LnH9VE4BtxR_Bf/view?usp=sharing)

*---An overview of the technology stack to be used---*

**Backend**
- <u>Django:</u> A high-level Python web framework for rapid development and clean, pragmatic design.

- <u>Django REST Framework (DRF):</u> A powerful and flexible toolkit for building Web APIs to work with Django.

- <u>Celery:</u> A distributed task queue for handling asynchronous tasks, used with Django for background processing.

- <u>Django Channels:</u> An extension to Django for handling WebSockets, enabling real-time data streaming and communication.

- <u>Redis:</u> An in-memory data structure store used as a database, cache, and message broker, primarily used with Celery for task management.

**Frontend & Wallet Integration**
- <u>React:</u> A popular JavaScript library for building user interfaces, particularly single-page applications.

- <u>Bootstrap:</u> CSS framework for responsive design and styling.

- <u>GrapeJS:</u> A web builder framework for creating HTML templates, styles, and components using a drag-and-drop interface.

- <u>MetaMask:</u> It allows users to access their Ethereum wallet through a browser extension or mobile app, which can then be used to interact with decentralized applications

- <u>Coinbase:</u> JavaScript SDK for interacting with Coinbase Wallet.

- <u>Walletconnect:</u> WalletConnect provider for connecting to Web3 compatible wallets.

- <u>Web3modal:</u>  A library for creating a user-friendly, Web3-compatible wallet connection interface.

**Database**
- <u>PostgreSQL:</u> A powerful, open-source object-relational database system with a strong reputation for reliability, feature robustness, and performance.

**Blockchain, Web3 & Smart Contracts**
- <u>Ethers:</u> JavaScript library for interacting with the Ethereum blockchain.

- <u>Ethersproject:</u> Utility functions for Ethereum address handling.

- <u>Solidity:</u> Solidity is an object-oriented programming language for implementing smart contracts on various blockchain platforms, most notably, Ethereum.

- <u>WebAssembly (WASM):</u> A binary instruction format for a stack-based virtual machine, used for compiling smart contracts.

- <u>Alchemy:</u> A powerful blockchain developer platform providing API access, developer tools, and infrastructure for Ethereum and other blockchain networks.

- <u>Haskell, Vyper, Rust, Go, Move:</u> Additional programming languages for smart contract development on various blockchain platforms.

- <u>web3:</u> Python library for interacting with Ethereum blockchain.

- <u>py-solc-x:</u> Python wrapper around the Solidity compiler (solc).

- <u>Cardano SDK, Near SDK, Cosmos SDK, Algorand SDK, Solana SDK:</u> Software development kits for integrating with their respective blockchains and working with smart contracts.

**Infrastructure, Deployments & Storage**
- <u>Docker:</u> A platform for developing, shipping, and running applications in containers, ensuring consistency across environments.

- <u>Alpine Linux:</u> A lightweight Linux distribution often used for Docker images.

- <u>NGINX:</u> A web server, reverse proxy server, and load balancer used for hosting and managing the frontend applications on their own subdomains.

- <u>Full Node Software:</u> Native Node Software for hosting nodes and managing validator engines unique to each chain (GoETH, Chain SDK’s etc).

- <u>nft.storage:</u> Client library for storing and retrieving NFT data on decentralized storage networks like IPFS.

- <u>Pillow:</u> Python Imaging Library for handling image files.

![Forward Factory Context Diagram](https://drive.google.com/file/d/12JVFDAPYsQG7Gh7cultEjHs4x6fmS_dl/view?usp=sharing)

*---Documentation of core components, protocols, architecture, etc. to be deployed---*

![Forward Network Context Diagram](https://drive.google.com/file/d/1mcJtjGV1KLiztmZMN1szytfXzD8U1JBz/view?usp=sharing)

*---PoC/MVP or other relevant prior work or research on the topic---*

- [Video Walkthrough of Forward](https://youtu.be/42RVRaizVl0)
- [Forward Factory Public Alpha (live)](forwardfactory.net)

### Ecosystem Fit

We have done a very detailed competitor analysis: [Forward Competion Analysis](https://docs.google.com/spreadsheets/d/1zRs810FL9DyaWVNq3NxOn3-bCMEcxKIZ2uBV6vz8fs4/edit?usp=sharing)

Let's discuss Moralis, Alchemy and similar platforms - they are developer assistant tools to help developers, they are not built for the end users with a zero code solution, so people could use Moralis and Alchemy to build applications, and put it in the Factory to scale to a non technical audience.

Forward is meant for the end user with a drag and drop no code application. 

There could be 100’s of different developers competing and having their own customized dApp templates in the marketplace for end users to deploy.

All of that is open, we are an open marketplace, where we’ll be transparently showing what is the number of deployment, reviews and ratings for users to make the best choice for themselves.

One of the other differences is that we use an EIP2535 at the heart of Forward Protocol. This allows a developer to update a specific function, they don’t have to update the whole contract, and they can push updates allowing a user to choose if they want to accept the update or not, just like WordPress where you get “update your plugin now”. This can be used to update contracts facet by facet, function by function, unlike a traditional proxy with a micro update functionality.

## Team
### Team members

- Karnika E. Yashwant (Co-founder)
- Mitch Rankin (Co-founder)
- Billy Weir (CTO)
- Zoe Fragou (Organizational psychologist)
- Rob Toth (Investor relations)
- Prashanth Konjerla (Collaborations)
- Danae Matara (Product manager)
- Adithya Thota (Project manager)
- 14 additional team members ranging from UI/UX designer to content creators.

### Team Website
- https://forwardprotocol.io - Product Details
- https://forwardfactory.net/ - Live product

### Team's experience
**Karnika E. Yashwant** - Co-founder
Karnika E. Yashwant (Mr. KEY) has been in the Blockchain space since 2013, founder of KEY Difference Media (KDM), the backbone to five of the top twenty blockchain marketing agencies, many US (SF/LA) based public relations (PR) & marketing firms. KDM has had clients such as CISCO, AJC, Fortune 100, eToro, ledger, and Verizon Media. (recommendations can be seen here https://www.linkedin.com/in/mrkey/) Mr. KEY is the ex-CTO of the NewsBTC Media Group (NewsBTC, Bitcoinist, LiveBitcoinNews, etc). He takes pleasure in 16 years of Content Marketing track record and 550m+ raised in ICO’s for various clients with a hybrid of technical, business and marketing experience.

**Mitch Rankin** - Co-founder
Mitch Rankin, is an entrepreneur, with 20 years of experience working with international investors. Co-founder English Forward, world's largest Learn English community with 310+ million users. 

**Billy Weir** - CTO
Billy Weir is Ex-Facebook and has expertise in Software Development and Engineering, Project Management, Fintech, Cryptocurrency, and experience in multiple niche sectors including Software development for Automation, AI, Adversarial networks, Data Science, Cryptography and many others.

### Team Code Repos

- https://github.com/ForwardProtocol
- https://github.com/billysweird

### Team LinkedIn Profiles

- https://www.linkedin.com/in/mrkey/ 
- https://www.linkedin.com/in/mitchrankin/
- https://www.linkedin.com/in/billy-weir-79b89a46 

## Development Roadmap

#### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3 | Milestone 4 | Total |
| - | - | - | - | - | - |
| Estimated Duration | 90 d | 180 d | 90 d | 90 d | 450 d |
| Full-time equivalent (FTE) | 2 | 1 | 1 | 2 | 6 |
| Cost (up to $ 25,000) | $ 2,500 | $ 10,000 | $ 10,000 | $ 2,500 | $ 25,000 |

#### Milestone 1 — On-boarding Developers, Marketplace templates and End-users

| Number | Deliverable | Specification |
|-|-|-|
| 1 | 840 developers building and uploading templates to the Forward Marketplace | We will provide MONTHLY updates on the 1st of every month showing the current stats. |
| 2 | Increase Forward’s Marketplace templates from 12 to 105 ready-to-deploy dApps. | We will provide MONTHLY updates on the 1st of every month showing the current stats. |
| 3 | 28,000 users using Forward Factory to deploy Forward Marketplace Templates. | We will provide MONTHLY updates on the 1st of every month showing the current stats. |

#### Milestone 2  —  Increase Forward’s internal development team to roll out new features faster
| Number | Deliverable | Specification |
|-|-|-|
| 1 | Forward affiliation system | Integrated into the Forward ecosystem and available to use.  |
| 2 | EIP 2535 (Diamond Contract Deployment)  | Integrated into the Forward ecosystem and available to use.  |
| 3 | Cross language auto conversion (Solidity, Rust, Go, Python, Move)  | Integrated into the Forward ecosystem and available to use.  |
| 4 | AI integration | Integrated into the Forward ecosystem and available to use.  |

#### Milestone 3  —  dApp deployments on VeChain through the Forward Factory
| Number | Deliverable | Specification |
|-|-|-|
| 1 | 200+ dApp deployments on VeChain | Metrics can be verified on-chain, we can provide a list of dApp contract addresses for you to check. This can also be verified through our API directly for authorized users once our API’s are made public.  |
| 2 | 20+ unique dApp deployments on VeChain  | Metrics can be verified by logging into the Forward Factory as a user/developer to see the templates in the Marketplace. We will also see if any API can be provisioned towards this data.  |

#### Milestone 4  —  Deployed dApp usage metrics on VeChain
| Number | Deliverable | Specification |
|-|-|-|
| 1 | 307,700 dApp transactions on VeChain (conservative estimate) | Metrics can be verified on-chain, we can provide a list of dApp contract addresses for you to check. This can also be verified through our API directly for authorized users once our API’s are made public.  |

#### Community engagement
- Medium: https://forwardprotocol.medium.com/ 
Forward will also commit to produce and publish an article/ tutorial to Forward’s Medium explaining the work Forward has done for the VeChain grant. 

On https://forwardprotocol.io/ we have provided the following links to our social media:
- Telegram: https://t.me/forwardprotocolofficial 
- Twitter: https://twitter.com/ForwardProtocol 
- Facebook: https://facebook.com/ForwardProtocol 
- Instagram: https://instagram.com/forwardprotocol 
- YouTube: https://www.youtube.com/forwardprotocol 
- Discord: https://discord.gg/X6HYF8dHYQ 

## Future Plans
- Integration of the Forward Network

## Additional Information
*---What work has been done so far---*

The Forward platform has already been built and is currently in Public Alpha. The Public Alpha utility includes building dApp templates with the no-code drag-and-drop interface, deploying dApps to 713+ EVM and Rust compatible chains, listing dApp templates on the open marketplace which can be deployed, integrated ticketing system, functionality to view your deployed dApps and interacting with the back-end, functionality to edit dApp templates that you have built.

*---Are there any other teams who have already invested in Forward---*

Pre-seed round investors:

Bleu Baggaley, Frank Papadakis, Mark Tolentino, Chaitanya, L Weitsz, Prasanth Konjerla, J Poupard, G Poupard, Chris Moller, Jarryd Moller, N Hind, C Peirson, Ramon Francis, Don Hill, A Wysall, G Fincham, T Harding, A Kippen, Mark Ball, Ryan Chandler Brown, Yaroslav Belkin.

Seed round investors:

Bitcoin.com, CVVC, MEXC (Exchange),X21,GDA Capital, Stakez Capital, Basics Capital, CRT Capital, ZBS Capital (CryptoDiffer), Magnus Capital, BlackDragon, Lotus Capital, MarketAcross, Buffet Investments, Darkpool Capital, Octopus Capital, NFT Technologies, Tokenova, Amesten, Polygon Syndicate, Ardura Capital, Utopian Capital, Cuan Ventures, Marathon Capital

IDO round investors:

Early community adopters through MahaStarter and DAO Maker

*---Have you applied for other grants so far---*

Optimism Builders Grant

Moonbeam Grants

IoTex Halo Grant

*---Forward’s detailed go-to-market strategy, including user acquisition channels and key target users---*

**GTM Strategy**

Forward Social Media: Marketing campaign using all channels.
- Social promotions
    - Organic Growth
    - Paid ads
- PR articles and content marketing with videos and blog posts
- AMAs with partners and unique guests
- Binance Live - Cast of users speaking about their use case and deploying their dApps with screen sharing

VeChain Collaboration: Co-marketing activities with VeChain 
- Forward Twitter post & RT to VeChain community,
- Forward PR article & blog post to Medium. If possible, Forward would like to have a featured PR article posted to the VeChain blog as well.
- Forward is open to AMA’s or any type of Web3 discussion with our founders:
    - KEY: https://www.linkedin.com/in/mrkey/ 
    - Mitch: https://www.linkedin.com/in/mitchrankin/ 

Start Affiliate Marketing Campaign 
- Using https://magic.store/ platform and their affiliate network for onboarding the first 40,000 users (under pay per acquisition contract with KPIs of dApp deployment, front end design and usage metrics)

List Forward on product directories: For onboarding early-adopters and product-feedback diversity
- AppSumo (Lifetime deal offered with discounted fees)
- BlockData
- Product Hunt (Promoting to be in Top 3 with ProductHunt growth marketing agency)

Use publications channels:
- Traditional PR channels and Crypto PR channels
- Cryptopolitan (Media Partner)
- Bitcoin.com (Investor)
- Binance Live (Publisher)
- Etc. (as seen on Forward Website)

Run contests:
- UI contest, for example: who can build the best front-end UI design using Forward.
- Giveaways, for example: Record and post a video while using Forward Factory.
- Bug bounties, for example: Be rewarded for finding bugs on Forward.

Hackathons:
- Developer hackathons with Dubai Blockchain Center, Jordan Web3 are in discussion. We are adding more hackathon partners to conduct and grow the developer base and templates.
- Business hackathons for business owners to come up with business ideas and use the Factory to bring it to life after learning the benefits of blockchain for their businesses. 
- Forward would also be keen on co-hosting a hackathon with the VeChain Foundation.

Engage with Developer communities:
- Build partnerships with current Dev communities and use their platform to promote the usage of Forward
    - ConsenSys developers (https://consensys.net/developers/) 
    - Alchemy University developers (https://university.alchemy.com/) 
    - LearnWeb3DAO (https://learnweb3.io/) 
    - WomanBuildWeb3 (https://www.30daysofweb3.xyz/) 
    - useWeb3 (https://www.useweb3.xyz/) 
    - BuildSpace (https://buildspace.so/)
    - DeveloperDAO (https://www.developerdao.com/)
    - Web3 University (https://www.web3.university/)
    - Surge Woman (https://www.surgewomen.io/web3-course)
    - H.E.R DAO (https://linktr.ee/H.E.R.DAO)
    - Pointer (https://www.pointer.gg/)
    - Web3 Career (https://web3.career/) 
    - Social Media Developer Influencers'
        - Julien Klepatch (https://twitter.com/jklepatch, https://eattheblocks.com/) 
        - Austin Griffith (https://twitter.com/austingriffith, https://austingriffith.com/)  
        - Patrick Collins (https://twitter.com/PatrickAlphaC, https://linktr.ee/PatrickAlphaC  
        - Nader Dabit (https://twitter.com/dabit3, https://nader.arweave.dev/)
        - Vitto Rivabella (https://twitter.com/VittoStack, https://vitto.cc/)  

**User Acquisition**

- Forward social media channels: 
    - Twitter
    - Telegram
    - Medium
    - Discord
    - Facebook
    - LinkedIn
    - Instagram
    - YouTube

- Partnered chains user and developer communities:
    - Polygon
    - Arbitrum
    - Avalanche
    - Optimism
    - Fantom
    - Cronos
    - Klaytn
    - Celo
    - Gnosis
    - KCC
    - Metis
    - OKC
    - Boba
    - Bitgert (BRISE)
    - AME Chain
    - zkSync
    - Reef
    - XDC Network
    - HSC
    - Chromia
    - Quai Network
    - Aurora
    - Moonbeam
    - RSK
    - IoTex
    - Syscoin
    - Kava
    - Telos

**Key targeted end-users and developers:**

Business owners, entrepreneurs, smart contract developers, web developers, web3 enthusiasts, businesses moving from web2 to web3. 

**Forward targeted Users: Users deploying through Forward Factory**

- Users/Projects that are aware of how Web3 can help them - Forward will be working with accelerators, incubators and VCs to on-board their portfolio projects, both traditional and crypto.
    - Businesses transitioning from Web2 to Web3.
    - Businesses that want to incorporate Web3 payments.
    - Web3 Entrepreneurs that want to build a Web3 business.
    - Web3 Enthusiasts that want to build and deploy dApps.
    - Web3 Projects that want to deploy on multiple chains.

- Users that are being educated via courses to be on-boarded - Forward will be publishing learning materials on how to effectively interact with Forward.
    - Non-technical Business Owners that want to build on Web3 and incorporate Web3 payments.
    - Non-technical Entrepreneurs that want to start a Web3 business.
    - Non-technical Web3 Enthusiasts that want to learn about Web3 and deploy dApps.

**Forward targeted Developers: Developers uploading templates to the Forward Marketplace**

- Experienced Developers
    - Web3 developers that want to monetize their project and template code.
    - Smart Contract Developers that want to monetize their smart contracts.
    - Front-end Developers that want to monetize their designs.

- Beginner Developers
    - Developers learning Web3.
    - Developers that want to deploy dApps quickly and easily.

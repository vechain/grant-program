# VeChain General Grant Application Template

## Project Overview 

- Project: Bazar. A marketplace to buy, sell and tokenizesustainable sourced products
- Team Name: Bazar
- Payment Address: 0x220a9ee5c3781d56b1292cbe71a1afd265fd44e4

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

<br />

Bazar is a marketplace aiming to decentralize the food supply chain and the logistics of trading sourced products. Inefficiencies in the food supply chain are accountable for 13 billion metric tons of CO2 emissions per year, plus fees, commissions, and lack of traceability of participants are draining the profits of small and medium producers limiting their capabilities of implementing sustainable practices. We found that many small and medium producers in Colombia and Brazil are choosing local brokers charging 10% to 15% in commissions to secure inventory purchases and sell their products to big stakeholders. Bazar stands for the basic principles of trade that have accompanied humans throughout history, which are freedom and transparency using the capabilities of blockchain, artificial intelligence, and IoT.

Our business model is based on removing the limitations that intermediaries present to producers in terms of fees and commissions, charging a subscription fee to Forwarders who are sitting to wait for customers to arrive in most cases. We measure impact with the most relevant features of our platform:
 
- Driving fees away from producers, allows them to invest these resources on environmental certifications and improvements to their production capabilities. 
- Integrating their existent IoT to Blockchain Technology allows us to measure CO2 capture more precisely. 
- Administrating producers' certifications and company documents allow us to connect them better with wholesalers interested in new CO2 Mitigation certified products
- Delivering Blockchain technology to the food supply chain will help to dimmish the over food waste problem of cargo in-transit
- Speeding the process of integration of forwarders to orders from buyers and sellers leads to successful transit of cargo and improvements of the overall supply chain logistics 
- Tokenizing the assets of farmers will give them an advantage over their competition in the long run

We are committed to contributing to a better future for the natural world, people, and economy something aligned with the VeChain principles. 

The most important functionalities for each partner of the network are defined as follows:

Producers or sellers:
- can upload their products
- modify smart contracts according to INCOTERMS (international trade terms) templates
- attach smart contracts to pre-defined commodity tokens (example: avocado token is a stable token)
- post their offers in the network
- stack tokens in their wallets
- convert tokens to fiat
- QR cargo (in-app feature)
- Choose forwarders (depending on initial INCOTERMS fixed by the buyer)
- Chat with network participants 



Wholesalers or buyers:
- can view the products on the network
- generate smart contracts according to INCOTERMS (international trade terms) templates
- top up their wallets with fiat and crypto
- chat with network participants 
- place bids for products
- admin smart contracts development (for shipping and insurance)
- choose forwarders
- QR cargo (in-app feature)

Forwarders/suppliers of services 
- post their services
- generate invoices (attachable to the ledger)
- QR cargo (app feature)
- view bids
- Chat with network participants when approved

A sample of our existent Hyperledger architecture is shown in this link, also described in the readme file of the Hyperledger repo.

For Artists we will create a space to post Digital Art based in 3D sampling of trees, animals, petroglyphs, and natural spaces that can be used in-game engines or simply as a way for people to support a good cause, 10% of the proceedings will be donated to rainforest alliance

- Create NFT's under the MetaForest guidelines
- Buy, Sell and Auction for NFTS's
- Transfer NTF's to other wallets 

Integration of VeChain features:
- Sync2: will allow users to manage their assets and transfer tokens from wholesalers to producers and from producers to forwarders
- Connex: will allow wholesalers to rapid buy items in the quantities they need from different network participants
- Thor: we think that the VeChainThor Blockchain can offer us an easy and trustworthy way of deploying our solution with more features than our hyperledger current development
TX Fee Delegation
- VeChain Cold and Carbon: in the long term we will be integrating IoT monitoring capabilities according to the readiness level of our costumers


<br /> 

### Project Details

#### Current assets/Stack (Work in progress)
* App (Flutter)
* Blockchain (Hyperledger Fabric, Phyton, NodeJS, GoLang)
* Escrow Crypto Wallet (Phyton, Solidity, ReactJS)
* Back-end (PHP)
* Data Base Structure (MySQL)
* API (NodeJS)


#### Mockups/Designs and UI components

* This designs illustrates some of the dashboard and app new functionalities for Buyers, Sellers and Fowarders, most screens are shared for all users and differs only on permissions inside the application. More screens are being designed as we test UX functionlities with peers
  * Dasboard
    ![Product Description for Buyers](https://github.com/Bazar-Network/mockups/blob/main/Dashboard/Buyer-product-dashboard.pdf)
    ![Overview of Wallet Dashboard for Buyers](https://github.com/Bazar-Network/mockups/blob/main/Dashboard/Buyer-wallet-dashboard.pdf)
    ![Products Management Page for Sellers](https://github.com/Bazar-Network/mockups/blob/main/Dashboard/Seller-product-dashboard.pdf)
    ![Products Management Page for Forwarders](https://github.com/Bazar-Network/mockups/blob/main/Dashboard/Fowarder-product-dashboard.pdf)
    ![General Screen for Customs Registry](https://github.com/Bazar-Network/mockups/blob/main/Dashboard/General-customs-dashboard.pdf)
  * App
    ![Updated Onboarding Screen 1](https://github.com/Bazar-Network/mockups/blob/main/App/Onboarding-1.pdf_1.jpg)
    ![Updated Onboarding Screen 2](https://github.com/Bazar-Network/mockups/blob/main/App/Onboarding-2.pdf_1.jpg)
    ![Updated Onboarding Screen 3](https://github.com/Bazar-Network/mockups/blob/main/App/Onboarding%20-3.pdf_1.jpg)
    ![Updated Phone Verification Screen](https://github.com/Bazar-Network/mockups/blob/main/App/Verification-code.pdf_1.jpg)
    ![New Trace Cargo Screen](https://github.com/Bazar-Network/mockups/blob/main/App/Trace%20Cargo.pdf_1.jpg)
    ![New Terms of Service Screen](https://github.com/Bazar-Network/mockups/blob/main/App/Terms%20of%20Service.pdf_1.jpg)
    ![New Suppliers Search Screen](https://github.com/Bazar-Network/mockups/blob/main/App/Suppliers%20search.pdf_1.jpg)
    ![New Products Log Screen](https://github.com/Bazar-Network/mockups/blob/main/App/Products%20Registry.pdf_1.jpg)
    ![New Payments Zone Screen](https://github.com/Bazar-Network/mockups/blob/main/App/Payments%20zone.pdf_1.jpg)
    ![New Cargo Status Screen](https://github.com/Bazar-Network/mockups/blob/main/App/Payments%20zone.pdf_1.jpg)
  * API Documentation 
    ![New Cargo Status Screen](https://github.com/Bazar-Network/API-Documentation/blob/main/API%20Documentation%20(in%20progress).docx)

* Tech Stack:
  * Phyton
  * NodeJS
  * ReactJS
  * Microservices Architecture
  * C++
  * My SQL
  * PHP
  * Solidity
  * Thor
  * Unreal Engine
* Network Architecture
  ![flow](https://github.com/Bazar-Network/hyperledger-bazar/blob/main/Architecture.png)

### Ecosystem Fit
Are there any other projects similar to yours? If so, how is your project different?

* So far there is no leading marketplace for trading sourced products under blockchain technology with integrated traceability, payments and authentication features, the closest example in terms of functionality is the IBM platform which is a centralized procurement SaaS solution for busineses and people that can afford its costs.
 
* Few SaaS solutions for the logistics industry are integrating IoT capabilities for in-trade opperations, VeChain features allow us to take Bazar to the next level of trade software 
 
* We can achieve new revenue models with VeChain and partners 

* Forwarders will be able to integrate their opperations to our marketplace therefore the VeCahin Blockchain

* Producer will be able to integrate existent IoT data to trades in the marketplace therefore to the VeChain network, increasing network usability

* We have collected a data set of 35,000 producers (73%), wholesalers (13%) and forwarders (14%) as we are continiusly expanding this we asked to 5% if they will be interested in a decentralized app to trade their products, the result was a 90% response positive (study is available, but information is sensitive to public share). 

## Team 

### Team members

- Esteban Marin, Developer, https://www.linkedin.com/in/estebanmarinramirez/, https://github.com/naturalesteban
- Kishor Parida, Developer, https://www.linkedin.com/in/kishor-parida-3961b875/, https://github.com/Kishor900
- Iván Martinez León, Developer, https://www.linkedin.com/in/iván-mart%C3%ADnez-león-12889336/
- Srikant Dash, Developer, https://www.linkedin.com/in/srikant-dash-341706a3/, https://kiger.renault.co.in/
- Nirrlipta Padhee, UX/UI, https://www.linkedin.com/in/nirrlipta28/, https://nirrlipta.wixsite.com/portfolio 

### Team Website

- https://bazar.network

### Team's experience

We have worked on other projects together, the most relevant was an application for a leading Bank in Latin America (https://www.bancolombia.com, description of the repo is included in this address https://campocredit@bitbucket.org/campocredit/auth-ids-service.git

Esteban Marin has over 15 years of experience in leading technical teams to successful prototyping and product development in diverse industries such as renewable energies, IoT, artificial intelligence, and financial services. He holds two patents in IoT and self-powered devices and has been awarded in international enterpreuship competitions. He also has attended international acceleration programs such as Startup Bootcamp and Techstars in past endeavors. Among his most important clients are Ferrovial and COLAS, both leading infrastructure firms in Europe; Bancolombia, Banorte, GNP, all leading companies in the financial services industry and the Colombian Government.  

Ivan Martinez Leon has 20 years of experience in building software for major banks, insurance, and marketing companies in Europe. He is currently working as a consultant for one of the leading software firms in Spain serving major banks and insurance stakeholders in the region. 

Kishor Parida is an entrepreneur with +10 years of experience and skilled qualifications in data science, applications programming, computer vision, deep learning, and gaming development. He has served as a consultant for important firms in the financial services in India.

Srikant Dash, is a programmer with +8 years of experience in building 3D environments for clients such as is Renault and Mahindra in India. He is very skilled in Unreal engine and python. https://kiger.renault.co.in/

Nirrlipta Padhee is a computer scientist and marketer expert in end-user-driven applications, her most important clients are Tech Majhindra, Mirriad, and Risk Management Solutions in the UK. Is a very skilled professional with an important background in programming and data science.


### Team Code Repos

- https://github.com/Bazar-Network/hyperledger-bazar<Hyperledger_Fabric_App>
- https://github.com/Bazar-Network/app-bazar<Flutter_App>
- https://github.com/Bazar-Network/escrow-wallet<Escrow_wallet>

## Development Roadmap 

As shown in the links mentioning past projects we follow best practices in code writing and deployment of applications this includes unitary tests for specific functions and applications, we also document the repositories improvements, modifications, comments, possible upgrades and follow a strict methodology to check that the code is well written, guides to run the application and detailed instructions of packages required to run the code. 

This project aims to deliver a working platform for managing products and orders, an app to view and interact with elements on the platform, designs of the resulting VeChainThor Ledger with a corresponding test suite, and a website (Marketplace) that will allow users to view products from the platform and create NFTs under the logic of MetaForest application


### Roadmap for a dApp Application

#### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3 | Milestone 4 | Total
| - | - |- | - |
| Estimated Duration | 30 d | 15 d | 15 d | 30 d | 90 d
| Full-time equivalent (FTE) | 2 | 1 | 2 | 1 | 6 
| Cost (up to $ 30,000) | $ 10,000 | $ 4,500 | $ 10,000| $ 5,500|

#### Milestone 1 — Trading Dashboard: Backend Integration and Frontend Development 

| # | Deliverables | Specification |
| ------ | ------ | ------ |
| 1 | User Authentication | Users will sign-up using the app alone (phone verification) then use a QR to sign-in into the trading dashboard |
| 1.1 | QR Authentication | Development for QR sign-in and for the registry and traceability of products to be sent by the seller to the forwarder and buyer |
| 2 | User Profile Management | Managing profile details of users on the platform |
| 2.1 | Documentation Manager | Upload of documents related to business operations, certificates, proof of business existence, etc. |
| 3 | Wallet | User can view their wallet balance, load the balance and create escrow accounts for trusted payments |
| 3.1 | Escrow Account | Buyers can create an escrow account to manage payments to sellers and forwarders, this also apply to buyers hiring forwarders services |
| 3.2 | Subscribe Bank Account | Buyers, sellers and forwarders can choose to use fiat money to perform trading operations |
| 3.3 | Connect Crypto Wallet | Connecting user to the crypto wallets (generating mnemonics etc.) |
| 4 | Logistics and traceability | Network participants can view the status of cargo in transit, smart contracts details, product details and ask for help |
| 4.1 | Location Services | Sellers and Forwarders can update status of cargo and automatically display them on a map|
| 5 | Product Manager | Upload products, manage inventory, smart contracts |
| 5.1 | Product Images | Upload images of products | 
| 5.2 | Inventory Manager | Create, delete, suspend, modify products |
| 5.3 | Smart Contracts Manager | Create, delete, suspend Smart Contracts |
| 6 | QR generator | Generate QR for added products |
| 7 | Products interaction | Network participants can view a detailed description of the products added by sellers and perform actions such as marking as a favorite, adding to cart, moving from cart |
| 8 | Reporting inappropriate | Reporting inappropriate or unethical listings on the platform |
| 9 | Product Reviews and Comments | Adding ratings and reviews for the products |
| 10 | Creating Marketplace | Creating a Digital marketplace dashboard for the buyers to interact with the products added by the sellers |
| 10.1 | Bid opportunities | Forwarders can view current bid opportunities to promote or appoint their services |
| 10.2 | Buy/Sell | Buy and Sell application, attach supplier (forwarder, insurance), choose Incoterms (Terms of trade), Contact/chatroom |
| 11 | Best products listed | Section for the best products like the most or better certified sourced products (Avocado with full suite of certifications) |
| 12 | Share links on different platforms | User can copy and share the link to sale item on different platforms |
| 13 | Integration of features to existent backend | Features will be integrated to existent backend |
| 14 | Frontend development and unitary tests | Screens, designs and testing |
| 15 | API development | Features are API'fied exposed and documented|


#### Milestone 2  —  App Improvements and integration to backend (The app wont integrate NFT’s)
| # | Deliverables | Specification |
| ------ | ------ | ------ |
| 16 | App Flutter Version Update | Current Stable App version is 1.20.1, desired version to update it is 2.8.0 |
| 17 | QR Module Update| QR sign-in, log-in and take a picture to register cargo |
| 18 | Products Screen | View, search products in-trade or traded, cancel, modify, increase size and suspend orders |
| 18.1 | Search Screen | Search products, suppliers, sellers and buyers |
| 18.2 | History Screen | View products traded and orders executed |
| 18.3 | Inventory Manager | Create, delete, suspend, modify products and smart contracts |
| 19 | Wallet Update | Update the screens to include crypto, escrow account and payments screen for buyers and sellers |
| 19.1 | Balance actions| Transfer balance, top up, admin escrow payments|
| 20 | Logistics Screen | Include maps and cargo process |
| 21 | Verification Update | Update verification module for users |
| 22 | Onboarding | Update onboarding screens for Buyers, Sellers and Forwarders to sign up | 
| 23 | Smart Contracts Manager | Create, delete, suspend Smart Contracts |
| 24 | Reporting inappropriate Screen | Reporting inappropriate or unethical listings on the platform |
| 25 | Product Reviews and Comments Screen | Adding ratings and reviews for the products |

#### Milestone 3  —  Blockchain Network Upgrade
| # | Deliverables | Specification |
| ------ | ------ | ------ |
| 26 | Migration | Migration from Hyperledger to Thor |
| 27 | Update Network Architecture | Add new features to network according to existent Thor documentation |
| 28 | Smart Contracts and Tokens Deployment | Build Templates according to INCOTERMS and Stable Tokens (There are 7 Templates) |
| 29 | Smart Contracts | Programming in Solidity of the Smart contracts |
| 30 | Tokens | Creation of tokens for first 6 sourced products (Avocado, Cacao, Corn, Beans, Timber, Coffee) |
| 31 | Price Feed Algorithm | The algorithm will extract the price from trusted commodity trading sources |
| 32 | Price Consensus Algorithm | The algorithm will create a consensus between the public price, the buyer desired price and the seller desired price |
| 33 | Testing | Unitary tests for functions, algorithms and the overall functionality of the network |

#### Milestone 4  —  Marketplace and MetaForest NFT’S in website for this Stage we will create two sections on the web version of the marketplace one for Sourced Products the other for MetaForest NFTS
| # | Deliverables | Specification |
| ------ | ------ | ------ |
| 34 | Backend Integration to Marketplace (Web) | API development for items available in the network to be displayed in the web version|
| 35 | Social Account Integration | Sign in using the Facebook and Twitter accounts (Only to view Sourced Products Items and Interact with NFT’s|
| 36 | Add NFT | Option to add artworks onto their account for sale/auction |
| 37 | Link NFT / Generate NFT Tokens | Generate/Mint the NFT for added products |
| 38 | Item interaction | Users can view a detailed description of the items added by the artist and perform certain actions such as marking as a favorite, adding to cart, moving from cart |
| 39 | Reporting inappropriate | Reporting inappropriate or unethical listings on the platform |
| 40 | Product Reviews and Comments | Adding ratings and reviews for the products |
| 41 | Featured Works | Section for the top artworks by relevance|
| 43 | Depositing NFT's from wallet and account | User can sell their NFTs bought from other NFT platforms |
| 44 | Share links on different platforms | User can copy and share the link to sale/auction item on different platforms |
| 45 | Auction & bidding | Other Users on the platform can start participating in the auction once started.
| 46 | Auction ending and result | The auction should end automatically when Endtime reaches and the highest bidder should be declared as winner (cron-job). Generation of results and basic analytics on auction end.
| 47 | Make an offer | Option to make an offer for the products added for Auction
| 48 | Get recent biddings | User can see and compare recent biddings
| 49 | Cart, favorites and owned | Option to view and manage the cart items, favorites, and owned NFTs on the MetaForest section
| 50 | Payment Process fro NTFs | Option to make the payment for the purchases of the Digital Artworks based notification | 
| 51 | Activity logs | To log the user Activity
| 52 | Notifications and manager | Option to control notification that is being shared with the end-users on the Digital Village platform
| 53 | Offer from other users | Users can view and accept offers from other users
| 54 | Manage ownership and resell | Option for the users on the Digital Village platform to resell their owned NFTs
| 55 | Royalties distribution| X% goes to the original product creator. 10% goes to Rain Forest Alliance. X% goes to the seller for secondary sales, X% goes to the creator, and the remaining X% goes to the platform.


#### Community engagement

A tutorial including videos, documents will be exposed in the website of Bazar. An article in medium will decribe the POC in detail with real users giving their feedback.

## Future Plans

We are in the process of raising funds with VC's and other investors mostly to send our developments to a production stage, maintain the code/platform, deploy marketing strategies with our growing data base of producers, wholesalers and fowarders and hire critical talent for the continuity of the business.

## Additional Information 

Any additional information that you think is relevant to this application that hasn't already been included.

Possible additional information to include:
- What work has been done so far?: We repropusing a propertary flutter app, back-end and API's that were designed as an application to grant credit in fiat to producers in the food supply chain. We also are in the process of building a data set of 35,000 producers (so far), wholesalers and fowarder from US, Colombia, Brasil, Peru and Nederlands
- Have you applied for other grants so far? Yes, we have applied to local grants in Colombia and successfull being awarded with ove 15,000 USD in cash and AWS credits that allowed us to continue the work and develop additional applications described in my github profile. We are also active in the NVIDIA inception program.

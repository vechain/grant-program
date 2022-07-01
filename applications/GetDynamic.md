# VeChain Grant Application for GetDynamic

## Project Overview 

- Project: GetDynamic Data Gateway & Messaging
- Team Name: AerodynamicData 
- USDT Payment Address: 0x8D4AA616E759058A9aD5cD4F43F4CbD23A7A6Baf


### Overview

GetDynamic is a web3 database connector for automation of B2B Data Exchange. Our app connects to existing on-prem and cloud based database infrastructure and allows pre-defined scripts to automatically send and receive data messages using a mix of peer2peer and blockchain technology. It is designed to be easy and quick to integrate for a selection of standard functions but also allows for complete customization. Beyond messaging Getdynamic also functions as a data-gateway for accessing emerging Web3 and Defi technology enabling business to accelerate data communication with its partners.

This project was inspired by Ryan Realivasquez's 15 years of experience as an ERP (Enterprise Resource Planning) Software consultant in the aerospace industry. Many companies have the same issues with data: How to quickly communicate important information with its business partners privately and securely. Most companies are still exchanging small amounts of data via phone and email or are using centralized systems at great cost. Existing messaging services have too high a cost of entry for small to medium sized businesses and offer little privacy. Many require aggregated data mining as a condition of service.  GetDynamic significantly reduces that transaction cost while protecting privacy and being transparent about what information is shared.  This results in data automation being available to a wider array of companies and accelerates business by pushing data to business partners as often as scheduled rather than a request handled via customer service.     

It's Free to Receive Data, It Saves Money to Send It. 




<p align="center">
<img src="https://user-images.githubusercontent.com/11070873/176514367-11f4b25f-4251-4ffa-821c-039061d87492.jpg" width="400" />
</p>

### Project Details
  
#### Infrastructure 
Our project is primarily based on Python, Django and Postgres.  Other technologies being used include Go, C#, Docker, Javascript, VMWare, IPFS, Truenas, and 
Cloudflare.  

#### Completed Development
Below is a technology overview of our webapp and what we currently have operational. 

<div align="center">
<table>
  <tr>
     <td>GetDynamic WebApp Overview</td>
  </tr>
 <tr>
    <td valign="top"><div align="center"><img src="https://user-images.githubusercontent.com/11070873/176323650-77de58fe-3bc7-4dc8-913e-9eec082ac246.png" width="200"> </td>
  </tr>
 </table>
 </div>


The following screenshots are from a working demo of the webapp (credentials provided to access demo): 
<div align="center">
<center>
<table>
  <tr>
    <td>Login Page</td>
     <td>Main Dashboard Page</td>
     <td>Add Company, Companies Page</td>
  </tr>
  <tr>
    <td valign="top"><img src="https://user-images.githubusercontent.com/11070873/168932198-c7ab7301-a457-403b-9293-2995e348d78d.png" width="200"></td>
    <td valign="top"><img src="https://user-images.githubusercontent.com/90410142/171931601-2adec06c-56b0-4c90-bab4-683640ebfa20.png" width="200"></td>
    <td valign="top"><img src="https://user-images.githubusercontent.com/90410142/171931601-2adec06c-56b0-4c90-bab4-683640ebfa20.png" width="200"> </td>
  </tr>
 </table>
 </center>
</div>
<div align="center">
<center>
<table>
  <tr>
    <td>Company List</td>
     <td>Send New Message</td>
     <td>System Configuration</td>
  </tr>
 <tr>
    <td valign="top"><img src="https://user-images.githubusercontent.com/11070873/168932731-1b1f08eb-4269-40b1-ad2e-36cbc2b49803.png" width="200" /></td>
    <td valign="top"><img src="https://user-images.githubusercontent.com/11070873/168932804-7240a274-6db7-4d64-8082-cb15bf0deeee.png" width="200"></td>
    <td valign="top"><img src="https://user-images.githubusercontent.com/11070873/168932902-4bf0df7c-4b5e-4601-b1e8-f018318260f7.png" width="200"> </td>
  </tr>
 </table>
 </center>
 </div>
 <div align="center"> 
<table>
  <tr>
    <td>
      Add Transaction Type</td>
  </tr>
  <tr>
    <td valign="top">
<img src="https://user-images.githubusercontent.com/11070873/168932979-6dde98f1-40c8-44da-91d9-6647f5cdf348.png" width="200" />
    </td></tr></table>
</div>


#### Functionality Overview 

#### Core Components:
GetDynamic consists of 3 core components: a Data Broker, a WebApp, and Smart Contracts.
The DataBroker handles the database setup and integrations allowing the definition and scheduling of automated scripts that send and receive data. It also shows a history of all decrypted data.   This app is designed to be installed locally inside of the client network.  
The WebApp manages all wallet and blockchain interaction and will conform at launch to web3 standards.   It keeps track of all encryption keys secured by the wallet as well as showing the history of all transactions sent and received.   This app can be installed inside the client network or can be accessed via our website.  (This component is currently operational) 
The SmartContracts manage all business logic.  Through Vechain VIP191 fee delegation clients do not have to hold their own crypto. Our smart contracts manage the authorization of transactions for fee delegation as well as hosting a public directory of users and initiating our privacy protocol for secure and private communications.   It also manages other functions such as key negotiation, IPFS private repository synchronization, and integrator commissions. 


#### Blockchain Functionality:
GetDynamic uses Web3 distributed ledger technology to integrate with the individual client company's wallet. The wallet connected to the app will contain hold all details of all wallets created and will be required to access transaction history. The wallet also works to control access to encryption keys.  For every company that a connection is made with new wallets are created and managed by the app. The app then completes a process to setup the automation and when ready begins automatically sending transactions based on the configured selection criteria. The data itself is not sent on the blockchain.  Rather a hash of the data is transferred.  This hash serves two purposes:  It validates that the data has not changed and also validates the location of the data. Please see the data exchange section below for additional detail. 

The web app and the wallets will interact with our smart contracts to validate transactions, manage public key exchange, coordinate IPFS configuration, as well as other features.  Please see the smart contract section for additional detail.


#### Data Exchange Functionality:  
GetDynamic is at its core a data gateway providing a pathway for data to safely and securely move between two companies.  To achieve this IPFS (InterPlanetaryFileSystem)  is used to exchange the data.  As part of our partner setup process a private data repository on IPFS is created and the key to access it exchanged. This ensures that both parties have access to the data at all times. 

After uploading the data to IPFS, GetDynamic sends a hash of the data to the partner. This hash performs 2 functions.   First, the hash validates that the data remains unchanged.  With the hash recorded to the chain, we can validate the data far into the future.  Second, the hash defines the location of the data on the IPFS network.  This 2nd function also supports the 1st function in that if the data changes, so does its location.  These features of IPFS and the immutable nature of the blockchain drives trust in the data and validates process quality.  If a company knows that transmitted data cannot be changed... they will ensure that the data being transmitted is accurate.  

#### Data Flow:  
The KEY to understanding the need for GetDynamic is that our app is designed to be connected to existing database infrastructure.   Companies will continue to do work in existing databases systems using their existing processes.   A big part of our growth is based upon building standardized integrations with those systems which will make it easy for companies to set up basic messaging for every day data exchange.  With standard integrations in place our client base opens up to ALL users of those database systems.   Epicor(Epicor.Com), Pentagon2000(Pentagon2000.com), Avsight(Avsight.Net), Quantum Control(ComponentControl.com)  and JobBoss(Jobboss.com) are 3 systems you can look at that we intend to integrate with. 

In the example below we show the data flow of a single automated data transaction.  In this case Company B ordered a widget from Company A.  Company A shipped the widget and recorded a ship tracking number.  That tracking number is then automatically sent to company B and ultimately written into their database.    So when the user at Company B goes to look in their database for the information on whether the widget has shipped or not... they see the already recorded shipping notification. 

  <div align="center">
<table>
  <tr>
    <td>
     Get Dynamic Data Flow Diagram Single Data Transaction </td>
  </tr>
  <tr>
    <td valign="top"><div align="center">
<img src="https://user-images.githubusercontent.com/11070873/176587352-2ee19e64-6f1f-4996-810c-d8cd61521c10.jpg" width="200" /></di>
    </td></tr></table>
</div>

 
#### API specifications of core functionality:
 An API will be built and published that integrates all core functionality (Sending and Receiving Transactions, Key Exchange, History Download, etc) as part of Milestone2.  
 
#### Decentralized Finance (DeFi): 
Currently defi functionality in GetDynamic is only in the planning stages. This is specifically because of regulatory uncertainty. With GetDynamic multiple types of financial transactions could automatically be created, executed, and recorded into company financial accounting systems.                         
Planned functionality includes: 

- Invoice payments - Invoices could be generated that would allow payment via crypto and settled in fiat.  

- Escrow - Payments can be structured to be based upon receipt and acceptance of invoice.  Multi-step payments could even be pre-configured based upon delivery milestones.  

- Deposits - For orders and released upon predefined criteria. 

- Leasing Contracts -  Payments and processing. 
 

### Use Case Scenarios: 
  Once configured our app is designed to be fully automated with minimal user interaction required. Below we provided 3 scenarios for one specific use case.   When an order is shipped, how is that information communicated from Company A to Company B via telephone, via email, or via GetDynamic. Similar use case scenarios are available for every day B2B communication like quote approvals, invoices, payment notifications, inventory updates, and more.  
Quite simply, GetDynamic does in a few seconds what companies are currently spending minutes on for every transaction. 
   
 
#### Shipping Notification Use Case Scenarios
<div align="center">

  
<table>
  <tr>
   <td>Phone</td>
    <td>Automated Email</td>
     <td>GetDynamic Automation</td>

  </tr>
 <tr>
    <td valign="top"><img src="https://user-images.githubusercontent.com/11070873/176323658-5df5b193-5428-45af-ad29-efd4d896216d.jpg" width="200"> </td>
    <td valign="top"><img src="https://user-images.githubusercontent.com/11070873/176323653-7c55aa62-e183-41cd-9be0-b333e3db39fb.jpg" width="200" /></td>
    <td valign="top"><img src="https://user-images.githubusercontent.com/11070873/176323656-402e033c-b597-46c6-9d28-bb0f2506e7d9.jpg" width="200"></td>
   
  </tr>
 </table>
 </center>
  </div>
  
  
  GetDynamic helps eliminate asynchronous  communication such as email and accelerates synchronous data communication to near real-time.  And it does this cheaper than any other company in the world. And by simply connecting to existing infrastructure rather than seeking to replace it GetDynamic makes it easy to automate exchange of data and deliver blockchain access.
  


<div align="center">
<table>
  <tr>
    <td>Create New Automated Transaction</td>
    
  </tr>
 <tr>
    <td valign="top"><div align="center"><img src="https://user-images.githubusercontent.com/11070873/176515613-86c1f0ae-9a00-4eab-a354-3cca0ce451a6.jpg" width="200" /></div></td>
    
  </tr>
 </table>
 </div>
  

### Smart Contract Functions   
Our smart contracts serve to manage the business logic of our system.  

<div align="center">
<table>
  <tr>
     <td>GetDynamic WebApp Overview</td>
  </tr>
 <tr>
    <td valign="top"><div align="center"><img src="https://user-images.githubusercontent.com/11070873/176323650-77de58fe-3bc7-4dc8-913e-9eec082ac246.png" width="200"> </td>
  </tr>
 </table>
 </div>

Below we have listed the key functionalities that will be supported by our smart contracts. 

- Wallet address registration:  This function will register new HD Wallet addresses that are associated with the primary wallet.  This will enable VIP-191 fee delegation to work with all associated wallets. 

- Transaction Payment and Processing:  As transaction requests are created this contract will upload the data to IPFS and will ultimately create a transaction that will send the encrypted IPFS hash to the designated receiver.	For any transactions received, the contract will decrypt the hash, retrieve the data, and pass it back.  This contract also validates payment from the sender's own wallet or via VIP191 fee delegation, or can draw tokens for transaction payment from the connected wallet if available. 

- Transaction commission:   Payment of commissions to the integrator who generated the new transactions is a fundamental part of the expansion of our app.  During setup an integrator can register a code.  That code gets transmitted with each transaction.  These transactions will be tracked and a commission will be paid to each integrator on a periodic basis as part of the contract. 

- Public Key Encryption Exchange: The smart contract will facilitate the exchange of public encryption keys to ensure that data is protected in transit and rest within the app. 

- IPFS Node Registration: For each data exchange partner an IPFS node, secured by an encryption key,  is created and maintained. The encryption key is required to access the stored data and is exchanged as part of the partner setup process.    

### Ecosystem Fit
Within Vechain no comparable projects are apparent. On other chains we have found messaging systems but have not found any that focus on connecting to existing corporate infrastructure for data exchange. Companies providing legacy Data Messaging systems include TrueCommerce, Seeburger, and IBM Sterling. Our app fits well within the Vechain ecosystem; it will provide an on-ramp for companies to leverage existing infrastructure in accessing and taking advantage of modern distributed ledger technology.

## Problems Solved by Blockchain 

The blockchain solves three problems for us:

- Trust and Transparency.     The structure of the system results in the immutable recording of a data hash that allows both sides to validate at any time that the data exchanged has never been changed.  The system also results in both parties having access to the exact same data and transaction history.  This provides a great reason for the sender to ensure that accurate data is always sent.  It also provides a great reason for the receiver to trust that the data the sender has sent is accurate.    

- Security and Privacy.      The blockchain offers a decentralized transport mechanism that allows two parties to directly exchange money and data.  Our system protects privacy and security by ensuring that all data is encrypted and is protected by the associated crypto wallet.   The system also protects privacy by generating new wallet addresses that are unique to each individual client relationship.  The system’s privacy protocol for establishing these channels results in transactions that have no discernable relationship with any information that is available on the public blockchain.  The details of the relationship only exist inside the app and are protected by the associated wallet.   All details required to access the data are encrypted at multiple levels and require access to the associated wallet to decrypt and view the data.  

- Cost.	Current systems charge fees based not only on transactional volume but also data volume.  Often transactions that generate higher data volumes come with greater cost. With GetDynamic there is a single standard transactional cost that does not differ with higher data volumes.  Discounts may apply based on transactional volumes.  This kind of data service has never been available at this low of a price point and thus opens the door to a larger number of companies using this kind of data service for a wider range of daily transactions.  

## Revenue Model 
Our app generates revenue via charging for transactions processed. Clients will be able to pay directly from their wallets via cryptocurrency but we expect that most clients will not want to hold their own cryptocurrencies.   For everybody else we will be offering monthly subscriptions with payment options in fiat currency. Subscriptions will allow for price variance based on volume and feature set. We expect 2000-2500 transactions per client per month with our standard transaction types.  

Revenue will also be generated from the professional services that may be required for modification of standard automation scripts as well as the production of custom scripts.  We also intend to generate revenue by providing data pathways to other services such as Inventory services, global shipping data, international customs compliance, and more.   


## Team 

### Team members & Contributors
- Ryan Realivasquez (Founder, Full stack Development) 
- Matt Haydon (Cofounder, Web Development, Marketing) 
- Genaro Coronel (Full Stack Development) 
- Oleg Tropinin (Full Stack Development) 

### Team Website

- https://getdynamic.app

### Team's experience

Ryan Realivasquez is the primary founder of GetDynamic. As an aerospace industry ERP consultant for over 15 years, he excels in implementing and supporting ERP systems. Through this experience he identified the need for a lower cost and more widely available system for exchanging data between companies. Utilizing the strengths of Blockchain technology he developed a simplified EDI system that addresses the needs of his clients and the industry overall. GetDynamic strengthens and improves upon existing EDI systems by focusing on three things: privacy, simplicity, and cost. Ryan launched development of the app, has researched and defined the infrastructure technologies to be used, defined the features and product roadmap, and has self funded the engagement of professional developers to complete initial development.

Matt Haydon is cofounder of GetDynamic. He has past experience launching several small businesses and is an influencer within the blockchain space, operating successful social media communities. Matt contributes to development of our app by focusing on interface design and building the User Experience(UX). Additionally, he develops future plans and continues to manage our web marketing plan.

Genaro Coronel is our principal developer. He has added several major features to the infrastructure of our app and will be our primary smart-contract developer as well. He is responsible for coding our IPFS-Cluster storage backend, dockerizing the infrastructure, and connecting the app to the Vechain network.

Oleg Tropinin has contributed to early development efforts and will be rejoining us for future development.  He has been responsible for our initial Vechain integration, web app infrastructure setup, and Django configuration.  



### Team Code Repos
Oleg Tropinin
https://github.com/olegtropinin

Genaro Coronel
https://github.com/genarocoronel

Matt Haydon
https://github.com/multidimensionalinteractive

Ryan Realivasquez
https://github.com/AerodynamicAutomatonff

### Team LinkedIn Profiles

- https://www.linkedin.com/in/ryanrealivasquez/
- https://www.linkedin.com/in/matthaydon/


## Development Roadmap 

### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3 | Milestone 4 | Total |
| - | - |- | - | - | - |
| Estimated Duration |Completed | 60 d | 60 d | 30 d | 150 d |
| Full-time equivalent (FTE) | 2 | 4 | 2 | 2 |
| Cost (up to $ 30,000) | $ 7,500 | $ 10,000 | $ 7,500 | $5,000| $ 30,000|

#### Milestone 1 — Infrastructure, Backend, WebApp, Website  

This first milestone represents work in-progress, tasks completed, and infrastructure costs for the next year. We request the foundation to please review our submitted work and validate completion of this 1st milestone. We are inspired to launch and this will allow us to move forward on completion of the remaining milestones.  

| 1a. | Infrastructure | Our goal is to secure funding for the first year of infrastructure service costs. Initially, this will cover a primary and backup VPS service each operating Vechain testnet and mainnet nodes, on-prem and cloud storage services for the network, data backups, and monitoring. Internal production and test network topology is configured for security with current generation enterprise quality gear.
- ISP Costs - Synchronous Gigabit Internet $150 per month
- VPS Costs -  2 VPS Servers @ $50 each per month 
- Hosting Fees - $50 Per Month
- Zoom Annual Team Subscription- $200 per year
- EV Wildcard SSL Cert - $200 per year 
- DataGrip Development and Collaboration Tools Annual Subscription (4 Licenses + 1 Extra) - $1625  

| 1b. | Backend | Our app is fully dockerized and ready for rapid stand alone deployment. Each major function is in its own container that can be managed separately. Containers include the ipfs daemon, a separate container for IPFS Cluster nodes, Postgres, Database Listener/Message Broker, Vechain node, and the web app itself running Django and Nginx. Repository documentation contains all details for launching the app however it simply can be built using 1. sudo bash build_project.sh and 2. docker-compose up -d . These two commands ran from the local repository folder will result in a functioning app ready for an account to be created and log in.

| 1c. | WebApp   |  Once containers are built and services started under milestone 1b, users are be able to login and access the webapp. The app itself focuses on showing the activity of data being exchanged, managing client relationships for purposes of data exchange, as well as integration with customer ERP database. Users will be able to send a manual message to validate functionality and on-chain transactions.

| 1d. | Website  |  Our primary website is currently active showing an explanation of our app, key details, and offers users the ability to request a demo. Software is online and we are ready to provide a demo.  Instructions to access demo are also provided in private repository. 


#### Milestone 2  —  API,  On-Prem Data Broker, Initial Data Scripts, Test Suite 

| 2a. | OpenAPI API Gateway | Create OpenAPI based api for performing key functions. API will be made available on RapidAPI. 
- Send New Transaction 
- Receive Transactions 
- New Exchange Request 
- IPFS Keyshare 
- History Download 
- Company Match 

| 2b. | On-Prem Data Broker | Middleware designed to manage the exchange of data between on-prem ERP database and the webapp.  This app will reside on 
the customer network and can be securely connected to the webapp's API interface to exchange data.   Data will be sent and received based on pre-defined and validated scripts.  This app, for this milestone, will connect initially to an oracle database.  Additional database types will be added in the future. 

| 2c. | Integration Scripts | The first integration scripts will be generated for this milestone.  These scripts will manage the import, export, and translation of data.  Initial operations to be covered include 
-Shipping Notifications -  Sends order number and tracking number 
-Shipping Detail - Sends Order number, tracking number, packing list, and any required paperwork.  
-Work Order Delivery Update - Sends order number, expected shipping date  
-Sales Delivery Date Change - Sends order number, expected shipping date 
-Invoice - Sends invoice details and creates an Accounts Payable in customer accounting system
-Payment Generated Alert - Sends notification a payment has been generated and details of payment (ACH/Check, Invoice#,  Date, Amount) 

| 2d. |  Test Suite   | -  We will develop a test suite to enable testing of all key functions including ERP database connections, sending and receiving transactions, and encryption/decryption processes.  



#### Milestone 3  —  Smart Contract 
| 3. | Smart Contracts | This milestone focuses on the creation and implementation of the smart contract that will drive the service.

| 3a. | Access Controls |  Control for VIP191 Fee Delegation vs Payment by Sender

| 3b. | Public Directory |  Public Authenticated Wallet Address Listing - An authenticated listing of public addresses will be created
to contact companies for purposes of this app.   This public address is only used for two purposes: To validate the company and initiate contact. 

| 3c. | IPFS Access Control - Keyshare for IPFS - As new client relationships are formed, clients have the option of using a shared IPFS swarm that all users subscribe to, or utilizing a private IPFS swarm shared only between two companies. The key to access each network share will be encrypted and exchanged triggering a new swarm to be created using the shared key.

| 3d. | Integrator Reward - Process to drive payment of a reward for transactions generated.  As transactions are generated an integrator ID code can be transmitted to indicate responsibility for generating these transactions.  A % of fees can then be directed to this integrator on a periodic basis. 



#### Milestone 4  —  I/O Script & ERP Integration Expansion, Documentation 
| 4a. | Data Import Export Scripts - We will expand the range of standard data scripts that we will support for each ERP integration.   

| 4b. | Additional ERP Integrations - We will expand our connection options to include a Microsoft SQL Server integration and a Salesforce Lightning integration.  Standard data import-export scripts will be built for each specific ERP system to simplify and accelerate client integration.  

| 4c. | Documentation - We will generate a full suite of documentation that details the process for setup, configuration, integration, and use of the software. Youtube videos will be created showing a walk through of the software and demonstration of key processes. Specifically, we will provide detailed instructions on how to create new import and export scripts to meet the user's specific needs.     

| 4d. | Transactional Support - We request the sponsoring of 100,000 VTHO.  These tokens will be used specifically for on-chain transactions by the webapp. With this support it will enable us to offer new customers an initial amount of free transactions to enable experience with the software and hopefully increase traction at no cost to the user. 


#### Community engagement
Medium Article - We will produce an article and publish it in Medium describing our app and its development as part of the program.   
Discord Server - A discord server is available at https://discord.gg/85qvDyrnZu. This will be a central place users can discuss the app, request support, and see feature announcements.
Community Events - We are active in the blockchain and startup communities in the greater Los Angeles/San Diego region.  We intend to openly discuss our app at various networking events and invite people to test it and consider building integrations for it.    
LinkedIN -   We will be using LinkedIN to reach out to our existing contact networks to share this tool and ignite interest. 
Tradeshows - As we gain traction we are prepared to attend and present at industry tradeshows for our targeted verticals.   


## Future Plans
The intention of our team is to use this grant to complete the buildout of our project and begin implementation with existing clients. With a small amount of traction we will add new features, increase the number of ERP integrations and begin recruiting a network of integrators who will bring online more companies using this tool. Our initial focus will be on manufacturing and service companies within several key markets. We also will look for opportunities to integrate with import-export businesses as well growth via partnerships with other software consultancies.

Our tool is a data-gateway for helping companies access new Web3/Defi technologies using their existing business management solutions. There are numerous opportunities for expansion in managing the exchange of data between companies. We will expand our standard data exchange offerings in areas of transactional data, audit controls, accounting/financial controls, and digital certification validation. We also intend for this company to be global in scale by serving and supporting B2B relationships across borders and overseas.

As our app grows we intend to validate our security, infrastructure and smart contracts through security audits. (Hacken?)  We also will seek to integrate Safehaven.io's solution's that will be attractive to corporate clients such as Safekey integration and inheritance.  

Opportunities for expansion into Defi abound as growth and regulatory compliance allows. 

Long term client expansion plans are focused on growth via native integration with ERP software providers, client word of mouth, and developing a network of IT firms, software consultants, and integrators who will be compensated for all transactions their integrations generate. 

We are committed to always creating more valuable transactions.



### [View our Pitch Deck](https://getdynamic.app/GetDynamic-App-Pitch-Deck.pdf)

[<img src="https://user-images.githubusercontent.com/11070873/176323652-b1428a83-d99c-4703-9cad-937e2ac96647.jpg" width="400"/>](https://getdynamic.app/GetDynamic-App-Pitch-Deck.pdf)

## Additional Information 

Our app is entirely self-funded and represents several years of discussion with clients, planning, design, and development work. Our vision is to find a way to better meet our clients needs at a lower price point than incumbent players utilizing other technologies. Vechain's platform, combined with other technologies, serves to meet those requirements. This is our first grant application. Our sincere goal is to build this app as a bridge to blockchain technologies from existing on-prem and cloud technologies.  

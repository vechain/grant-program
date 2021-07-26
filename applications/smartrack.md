# VeChain General Grant Application Template

## Project Overview 

- Project: Smartrack.io
- Team Name: Smartrack.io
- Payment Address: 0x2847b5372201318Ea65d5Df9E648DC509e59fe21

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Project Overview
- Project description: Blockchain based recordkeeping for inventory and service records for equipement leased and sold to customers on their work sites

In many electronics industry segments, the up-front capitol cost of installing electrical systems is only the beginning of the expenses associated with the equipement. The maintenance and updating of these systems over time can be a significant portion of the total cost of the system. One of the most time consuming aspects of this maintenance can be the simple task of retrieving records and documentation for the equipement, especially since these records must be accessible and modifiable by third party contractors. At this time, services that store and make this data accessible are subject to a monthly costly subscription. Oftentimes, once the subscription is cancelled, the data will no longer be accessible. This high cost and data impermanence make these services impractical for small businesses. Therefore, there is a market need for affordable, permanent, and easily accessible records for inventory and service records for equipment on customer work sites. Our Smartrack VeChain project will address this stated market need. 
	
Smartrack is an dApp for inventory and service record tracking on the VeChain blockchain that will allow small businesses to upload their data to the public blockchain with a one time gas fee, eliminating the need for expensive subscription services. Each installed piece of equipment at the customer's site will be uploaded as a "rack" that is associated with a "company" in the system. This "company" will be associated with a public wallet which will pay the gas fees for the upload of service records and act as an organizing node within the system to tie all of the tracked "racks" with the host company. The customer's "rack" data will be easily accessible and updateable through a QR code located on the device being tracked. 

VeChain is an ideal platform for this application due to its stable gas prices, fast transactions, fee delegation, forceable transaction dependency and multiple clause transaction features. The stable gas prices will allow for use in enterprise applications by providing precise expense forecasting associated with maintenance documentation, while the fast transaction speeds will ensure contract maintenance workers are not hindered by slow systems. Fee delegation will allow the "company" who owns the "rack" to cover the gas fees for uploads, meaning the third party maintenance workers will not need to have any direct knowledge of the blockchain in order to upload data to it. Forceable transactions dependencies will ensure no gas fees are wasted if a multi-transaction file upload fails during one of the upload sections, allowing users to upload light product documentation effectively. Finally, multiple clause transactions will allow users to upload data for multiple "racks" in a single transaction in order to optimize costs.
	
- Integration of VeChain Tools and Features
	- The dApp is serverless. The front-end web application only connects to the blockchain for data storage and manipulation. No other database is required.
	- The dApp is an interface to the Vechain blockchain using the Sync2 wallet to identify individual users holding company ownership (using a cert) and to pay for fees to create "companies" and "racks".
	- Connex2 is used as a part of the back-end of the website to interact with the blockchain.
	- The dApp offers fee delegation in the smart contract options.  Companies can allow third parties to write service reports to a "racks" contract while using gas fees delegated by the company.
	- The dApp implements Multi-task Transaction ("MTT") as a way to add multiple devices to a "racks" inventory in a single transaction.
	- The dApp impliments Forcible Transaction Dependency to store files larger then allowed in one transaction. This will allow users to supply light documentation associated with the tracked hardware.

### Project Details

We provide the following project information for consideration:

- Mockups/designs of any UI components\
	https://github.com/thejoshstoll/smartrack-ui-screenshots
	
- API specifications of the core functionality
	- Creation of ID based on public wallet address (mappings based on that). This company ID based on public wallet ID to act as mapping point for all uploaded data.
	- Create and Update a "Main" contract that indexes all information stored on a per company basis.
	- Create and Update racks on the blockchain.
	- Mark racks as invisible. (Racks cannot be truly deleted from the block chain.
	- Create, Update and Delete devices on a rack.
	- Create services records on a rack.
	- Encrypt and Decrypt data stored on the blockchain.
	- Creation of GUID's and matching QR codes to place on racks, for identification and access to rack information.
	- Allow for third parties to Get and Update racks on the block chain at the descretion of the racks owner.
	
- An overview of the technology stack to be used\
Smart contracts: Truffle\
Encryption: Stanford Javascript Crypto Library\
Front-end/Back-end: React App/Angular for front end. Backend will be ISS server, only to serve front end web app.

- Documentation of core components, protocols, architecture, etc. to be deployed

We will deploy a smart contract that allows end users to create a company, index customers, and find "rack" address locations (these are smart contracts deployed from the main smart contract) on "rack" creation.\
This data will be accessed via our UI hosted on smartrack.io
	

- PoC/MVP or other relevant prior work or research on the topic
	- https://github.com/thejoshstoll/smartrack-poc
	- We have a working POC on the Vechain Testnet address: 0x7fA00bbc66aa4796fab037B1aDb94094F6a98E35
	- https://explore-testnet.vechain.org/accounts/0x7fa00bbc66aa4796fab037b1adb94094f6a98e35/

### Ecosystem Fit
We are not aware of any similar projects. Therefore, we belive Smartrack has the potential to expand the real world application of VeChain and raise its profile in the broader market place.

## Team 

### Team members

- Name of team leader\
	Joshua Stoll
- Names of team members\
	Josiah Taves\
	Marcus Haberling

### Team Website

- https://smartrack.io

### Team's experience

Joshua Stoll - A Programmer at Video Pro in Brisbane, Australia. Responsible for creating UI's and programming for AV integration for corporate clients, University classrooms, and government facilities.

Josiah Taves - An Electrical Engineer at Alderon Industries in Minnesota, USA. Responsible for designing electronics for commercial and industrial wastewater control systems, programming the embedded systems contained therein, as well as supply chain management for the production of these systems.

Marcus Haberling - A Software Engineer at Alderon Industries in Minnesota, USA. Responsible for the design, immplementation, and maitnence of an "Internet of Things" cloud platform as well as internal process improvement software.

We are unable to produce any repositories of previous works on github as these are owned by our employers.

### Team Code Repos

- Project Repo: https://github.com/users/thejoshstoll/projects/2
- Joshua Stoll: https://github.com/thejoshstoll
- Josiah Taves: https://github.com/josiah-taves
- Marcus Haberling: https://github.com/haberling


### Team LinkedIn Profiles

- Joshua Stoll: https://www.linkedin.com/in/joshua-stoll-061533115/
- Josiah Taves: https://www.linkedin.com/in/josiah-taves-228186216/
- Marcus Haberling: https://www.linkedin.com/in/marcus-haberling-9053491a8/

## Development Roadmap 

We provide the below as a roadmap to the milestones to be achieved at each stage of the development. It is anticipated the completion of this project will take 150 days. We provide further detail of this breakdown below.  

#### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3 | Total |
| - | - |- | - | - |
| Estimated Duration | 50 d | 50 d | 50 d | 150 d |
| Full-time equivalent (FTE) | 2 | 2 | 2 | - |
| Cost (up to $ 30,000) | $ 10,000 | $ 10,000 | $ 10,000| $ 30,000|

#### Milestone 1 — Smart Contracts, Test Suite, & Tutorial

| Number | Deliverable | Specification |
|-|-|-|
| 1| License | Apache 2.0 / MIT / Unlicense |
| 2a | Smart Contract Creation "Main"| Main smart contract that will index all contracts on a company basis|
| 2b | Smart Contract Creation "Company" | Smart contract that will create customers and track customer smart contract location|
| 2c | Smart Contract Creation "Customer" | Smart contract created by "Create Customer" to track customer rack locations |
| 2d | Smart Contract Creation "Rack" | Smart contract that will be created by "Create Rack" contract to represent a rack location |
| 2e | Documentation | We will provide thorough inline comments in the smart contracts |
| 3 | Smart Contract Testing Suite | Create unit testing suite |
| 4 | Smart Contract Testing Guide | In the guide, we will describe how to run these tests |
| 5 | Smart Contract Deployment | Smart contracts deployed to Vechain testnet |
| 6 | Smart Contract Tuturial | A basic tuturial on how to create smart contracts for Vechain in Remix |
#### Milestone 2  —  Backend, Company Encryption, & Tutorial

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Backend | We will create a backend service that will allow recall of company’s data |
| 2 | Documentation | We will provide inline documentation to the backend code |
| 3 | Encryption Implementation | Enable encryption on a company level |
| 4 | Backend Tutorial | We will provide a basic tutorial to provide other users the ability to create a simple react-app and use this to interact with a smart contract on the Vechain network|
#### Milestone 3  —  Frontend, Rack Encryption, & Tutorial

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Encryption Implementation | Enabling encryption on a rack level in a way that both the master pincode of the company and the pincode of the rack can access the rack data |
| 2 | Backend | We will create a backend service that will allow recall of rack information |
| 3 | UI |We will develop a clean looking UI with Home page, company owner page, admin page, and Rack View page |
| 4 | Front-end/Backend| Integrate front-end to backend |
| 5 | Documentation | We will provide inline documentation to the front-end code |
| 6 | Smart Contract Deployment | Smart contracts deployed to Vechain mainnet |
| 7 | Implementation Tutorial | We will provide a thorough tutorial to give other users the ability to manipulate and deploy our contracts and backend/front-end for other industry needs to nuture growth of transactions on the Vechain blockchain |
| 8 | As Built | On the Github repository, commit a compiled (ng build) version of the Angular front end and smart contracts that can be quickly deployed by anyone in the VeChain community

#### Community engagement

Our project will be an engagement piece for numerous stakeholders and interested parties both within the technical community and general end user community. We will produce numerous tutorials (as outlined above) to be published on the Medium website for the greater community to utilise. It will create a compelling and broad-reaching bridge between end users and the Vechain platform by enhancing their experience with blockchain technology and creating an application that can be widely used. 

Additionally, we will be active on Vechain's Reddit providing updates and responding to any questions about the project, creating a continued interest in how the platform can serve end user needs. We consider interviews and demonstrations with Vechain influencers to be another avenue for our exploration.  


## Future Plans

Ultimately, it is our plan to maintain an active website and continue to provide support for companies and app developments to integrate Vechain technology. This is achievable due to the low overhead cost and small fee to be charged to users for the creation of the "rack" smart contract. Given the ability to maintain an active website is attainable, it is within our ambit to explore other market opportunities to implement our project. The Smartrack application will be able to adapt to numerous industries looking for sustainable, editable and an end-user friendly experience. To start, over the next year we intend to develop modules for hardware controllers used in commercial AV integration (AMX, Crestron, Extron) that would be able to interact with the smart contracts and report faults. Overall, we consider the adaptability of this project ought to be highly regarded as a gateway to decentralized applications.    


## Additional Information 

- What work has been done so far?\
We have a current working demo on the Vechain testnet.

- Are there any teams who have already contributed (financially) to the project?\
At this stage the only cost has been the website domain. 

- Have you applied for other grants so far?\
There have been no other grants applied for. 

- Joshua is an economic strength node holder.
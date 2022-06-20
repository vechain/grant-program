# VeChain General Grant Application

## Project Overview 

- Project: VOTEOS
- Team Name: HPM GmbH
- Payment Address USDT: 0xd450dabfb20cd5294c76eea0ec80c3ca34c3437a

### Overview

VOTEOS is an audit-proof voting solution aimed at corporate users.

Management boards and other decision-making bodies usually have to vote on decisions at regular intervals. The requirements for the formal procedures of those meetings are regulated by law.

In the wake of the still ongoing pandemic situation, the demand for a digital solution for voting processes has increased rapidly. Even though the legal requirements have been reduced somewhat, the challenge remains to have a digital and remote voting process which adheres to law from start to finish.

VOTEOS aims to be an all in one platform for digital voting. Starting with the registration and ending with election results, the whole process happens digitally on the blockchain.  
  
VeChain was chosen due to the fee delegation feature, as it allows us to provide our service to customers without prior blockchain experience.

### Project Details

Everything relevant to the voting process is stored and managed by smart contracts. Private data is encrypted and saved in IPFS and can only be accessed by organization members.

**What does it solve?**

Currently, there is no legally secure method for digital voting.

With the help of blockchain technology, votes and election processes can be mapped in an audit-proof manner.  
  
This leads to the core features:

- Revision security
- No registration requirement for voters, easy on-boarding for voting
- Data protection compliant
- Real-time evaluation
- Transfer of votes
- Simple administration and payment
- Privacy protection law compliant

**Who will use it?**

The Audience includes all groups that, for reasons of civil or commercial law, are required to perform and document legally compliant votings.

**Where can I use it?**

The most common use cases are:

- Bringing about solutions to amend bylaws and contracts.
- Election of supervisory boards, management boards and other positions
- Discharge of management or board of directors 
- Voting on motions from the auditorium.
- Elections at owners' meetings
- etc.

**Infrastructure in a Nutshell**

Technically contracts will be deployed for each election and votes will be minted as NFT. Using the NFT standard allows potential integration with other wallets/applications/platforms. Tokens can be shared and used for voting. All metadata is stored on IPFS, with a on-the-fly-encryption within a custom ipfs proxy that enforces access control managed in smart contracts.

IPFS Proxy and Website-UIs are hosted on AWS. Providing an IPFS or distributed version is planned for the future.

#### Organizer Application flow

```mermaid
sequenceDiagram
    autonumber
    actor Organizer
    participant Organization
    participant Election
    participant Voter Registry
    actor Voter
    Note over Organizer,Organization : Setup new Organization
    Organizer->>Organizer: Sign Up
    Organizer->>Organization: create Organization
    Organization-->>Organizer: invite more Managers
    Note over Organization,Voter Registry: Setup new Election
    Organization->>Election: create Election
    Election-->Voter Registry: link Voter Registry
    loop configuration
      Voter Registry-->Voter Registry: manage Voters
      Election-->Election: manage Polls
    end
    Organizer->>Voter Registry: mint Votes for each Voter
    Voter Registry-->>Voter: provide Votes
   
    Note over Organization,Voter: Election
    Voter-->>Election: Vote on Polls
    Election-->>Organization: Provide results
```

#### Vote provision flow

```mermaid
sequenceDiagram
    autonumber
    actor Organizer
    actor Voter
    participant Election
    participant Voter Registry
    Note over Organizer : prepare
    Organizer->>Voter Registry: Manages
    Organizer->>Election: connect Registry
    Organizer->>Organizer: generate Wallets 
    Organizer->>Election: generate Votes
    Election->>Organizer: Votes
    Organizer->>Voter: send Vote to Individual Voter
    Note over Voter,Election: participate
    Voter->>Election: Vote on Polls
    Election-->>Voter: provide results
    Election-->>Organizer: provide results
```


#### Application Screens

**Admin Dashboard to organize Votes**   

* ![VOTEOS_Dashboard](https://chat.hpm.agency/files/p8o65qrgkbrr3rdcecest8x67r/public?h=ekkMvTVx3VI1XoI15b8zbUeywpA7c1L4FQv8n4dcolI)
  
**Create a Question**

* ![Create_Polls](https://chat.hpm.agency/files/k1ik4h88sig4defbq1bdicxiky/public?h=t3N2-zdtssw4xXWCklq22MDaEKOb884t93L5E_APrU4)
  
**Manage the Agenda**

* ![Create_Agendas](https://chat.hpm.agency/files/d3risxeq3fdb3ynfxtrhehwi9e/public?h=fOlIdWqIW_pp2nyphLpwAcIP5C67rHG6XzS3Wq7NHgw)
  
**Add Voters**

* ![Create_a_Voter_Registry](https://chat.hpm.agency/files/6pxx86ojpt8p5m4q69x9hzrkaa/public?h=SssBqH2_ELKyS_UXy5WOJFitRYrgv7vdu2a1-pJAatk)
  
**Create Votes**

* ![Create_Votes](https://chat.hpm.agency/files/8cx4mfjrbpd47k83yrfo7mhjsc/public?h=73BriF2_z-agD8GTZKABLnmqY-U0Q9HVUNFalcB5JYI)
  
**Election Moderation**

* ![Navigate_through_live_events](https://chat.hpm.agency/files/1f1f4hujitf8jnyipk37ghzmew/public?h=KJwGa9xtqv0VL4I9wlooujRe2XNj8_fUUcHw8SJfeW8)
  
**Join Election on Mobile**

* ![Ballots_Count](https://chat.hpm.agency/files/k3fy1f1b7ibxmffmsrrugdioho/public?h=bnJbdd7L3hjCOP27KuAQiV_hA-mwCdp3IZGWWAerWeQ)

**Vote on Mobile**

* ![Vote](https://chat.hpm.agency/files/gngwuxyomj8u78b9697x1thpcy/public?h=Q_q0dO6fDo26gXA4_ZFTaHbfXen9bTBW0n_3UlNQ7yc)

**Results on Mobile**

![Mobile_Results](https://chat.hpm.agency/files/6ej3dps8qidn9ndktn9raundxr/public?h=WKpeO6mvbkJwnJr-M38mXrw5BGh-1raej9LeC1hlNHs)

**Presentation View**

* ![View_for_Presentation](https://chat.hpm.agency/files/3k5ki9174bd6my9sta4uwszyyc/public?h=Vnp6ktTKeGyL4cxNGDAh27NvOQX_zNlgPoYZsAxgesg)

#### Tech-stack

The UI is built using React, Backend-Services to provide encrypted IPFS data are built using NodeJS. Pinata is used to support storage on IPFS.

* Frontends
   * Admin, Voter and Presentation
   * Ant Design Components
* Wallet
   * toruslabs/openlogin
   * social login
* Backend
   * IPFSproxy for Pinata
      * used for metadata and file storage
      * to encrypt end decrypt private data
   * NodeJS Backend
   * hapi framework
* Blockchain
   * Contracts
   * Hardhat development environment

```mermaid
flowchart
  subgraph Frontends[Frontends]
    direction TB
    AdminFrontend[Admin Frontend]
    VotingFrontend[Voting Frontend]
    PresentationFrontend[Presentation Frontend]
  end

  subgraph Blockchain
    Contracts["Contracts"]
  end

  subgraph Wallet
    web3auth[Web 3 social auth]
  end

  IPFS["IPFS Pinata"]

  subgraph Backend
    direction TB
    IPFSProxy["IPFSProxy"]
    voterRegistry["Voter Registry"]
  end

  Frontends --- Backend
  Frontends --- Blockchain
  Frontends --- Wallet
  Blockchain --- Backend
  Backend ---   IPFS
```

## Access control

```mermaid
sequenceDiagram
    actor User
    participant voteos
    participant Backend
    participant Contract

    note over User, Backend: Initialize Session
    User->>Backend: request session
    Backend-->>Backend: create JWT Session
    Backend-->>User: respond with session JWT

    User-->>User: sign JWT with private Key

    note over Backend, Contract: Session Validation
    User->>Backend: send JWT + Signature + Contract Address + Data
    alt is valid Signature for valid JWT

       Backend->>Contract: read user role
       Contract-->>Backend: user role

       alt is Allowed
           Backend-->>User: respond with data
       else is Unknown
           Backend-->>User: Error
       end

    else is invalid Signature
        Backend-->>User: Error
    end
```

### Ecosystem Fit

- It is an ecosystem enrichment as it is the first of its kind
- This project generates attention from corporate customers for VeChain
- We introduce _users unfamiliar with blockchain technology_ to the ecosystem

## Team 

### Team members

- 8 Team members of HPM GmbH

### Team Website

- https://hpm.agency/
- https://admin.voteos.com/  (Preview-Version)
- https://voteos.com (Preview-Website, currently german only)

### Team's experience

Our whole team is currently 15 members strong and is building enterprise applications for more than 20 years. Building custom solutions for enterprises and re-useable products is our daily business.

### Team Code Repos

- No public Code Repositories available
- Access to private Repositories and more detailed documentation can be granted under NDA

## Development Roadmap 
#### Overview

|                                  | Auth-Workflow | Election Administration | Voter Administration & Vote Distribution | Voting & Results | Payment |         |
|----------------------------------|---------------|-------------------------|------------------------------------------|------------------|---------|---------|
| Duration                         | 2             | 8                       | 8                                        | 9                | 4       | 33      |
| Full-time equivalent (FTE)       | 1             | 2                       | 2                                        | 2                | 4       | 11      |
| Cost                             | $880          | $7.040                  | $7.040                                   | $7.920           | $7.040  | $29.920 |

Based on a $440 / daily rate. $1200 is the normal rate which is covered by HPM.

#### Milestone 1 Auth-Workflow & Setup

| Number | Deliverable       | Specification                                                                                      |
|--------|-------------------|----------------------------------------------------------------------------------------------------|
| 1      | Auth-Workflow     | Sign Up/-In with web3auth for hosted wallets |
| 1.1    | Integrate service | Web3auth toruslabs/openlogin for passwordless login                                               |
| 1.2    | Session Micro-Service | Create micro-service for session handling and access protection                                                         |


#### Milestone 2 Election Administration

| Number | Deliverable             | Specification                                                           |
|--------|-------------------------|-------------------------------------------------------------------------|
| 2      | Election Administration | -                                                                       |
| 2.1    | Organization Management | Create and edit Organizations in admin frontend                         |
| 2.1.1  | Membership management                  | Manage Organization Members, Member invite & join                       |
| 2.1.2  | Audit Log               | Organization audit log using Blockchain events                          |
| 2.2    | Election Management     | Create and manage elections in admin frontend, including live execution |
| 2.2.1  | Attachment handling     | Allow adding file attachments hosted in IPFS                            |
| 2.3    | Poll Management         | Create and manage questions                                             |
| 2.3.1  | Answer Management       | Create and manage answers                              |


#### Milestone 3 Voter Administration & Vote Distribution

| Number | Deliverable                              | Specification                                                                                        |
|--------|------------------------------------------|------------------------------------------------------------------------------------------------------|
| 3      | Voter Administration & Vote Distribution | -                                                                                                    |
| 3.1    | Voter Registry                           | Create Voter Registry for potential voter with encrypted data only accessible to organization members |
| 3.2    | Vote-Distribution                        | ERC-721 NFT Vote minting and distribution, CSV download of created votes                             |    

#### Milestone 4 Voting & Results

| Number | Deliverable         | Specification                                                                                           |
|--------|---------------------|---------------------------------------------------------------------------------------------------------|
| 4      | Voting & Results    |                                                                                                         |
| 4.1    | Join Event and vote | Voting frontend, join an election by link, vote on active polls                                         |
| 4.1.1  | Private data        | Access private data with an ipfs proxy that encrypts/decrypts on the fly with access validation for the smart contract organization members |
| 4.1.2  | Vote Sharing        | Ability to share votes (Tokens) and cast (multiple) votes for other users |
| 4.2    | Results             | Display results to all parties                                                                          |
| 4.3    | Presentation view   | Read only presentation view for broadcasting (optimized for crowd viewing)                                                                             |


#### Milestone 5 Payment

| Number | Deliverable         | Specification                       |
|--------|---------------------|-------------------------------------|
| 5      | Payment             | -                                   |
| 5.1    | Service Integration | Stripe payment provider integration |
| 5.2    | History             | Organisation purchase history       |
| 5.3    | Refund              | Ballot refund administration        |

## Community engagement and marketing

Our main marketing statement consists of creating and running audit-proof elections in a simple and uncomplicated workflow - _"as easy as sending a text message"_.   
In order to brand awareness for VOTEOS and VeChain we are planning to run marketing campaigns on social media and business networks.   
Additionally articles on the conduct of various types of elections will be published to digital platforms like [Medium.com](https://medium.com/).   
By giving away free packages of votes, we can lower the entry barrier to our service.  
Our initial sales strategy will be to acquire users through direct marketing in the founder's personal business network of entrepreneurs and employees in management positions.

## Future Plans
Our goal is to create a digital voting solution for associations and companies. Our premise is to allow anyone to simply create and conduct audit proof elections at reasonable cost. We will keep on developing features and optimizations to establish blockchain voting in the target group.

### Planned features include
- Voting weights
- Poll templates / export + import
- Performance and cost monitoring
- Vote burning
- Result export

## Business Model

Billing is based on the "pay per use" principle. Each ballot costs a certain amount. Ballots are bought by organizers for organizations.

- [Stripe.com](https://stripe.com/) is used as payment service provider
- Sale of ballots
  
| Ballot range | cost/ballot |
| ------ | ------ |
| Up to 100 | 2€ |
| 101 - 500 | 1,50€ |
| 501 and above | 1€ |

## Additional Information 

* To this day we have already managed to carry out a prototype election together with the `Initiative Deutsche Zahlungssysteme`
* HPM GmbH funds the development out of its own resources right now
* We have not applied to any other grants
  

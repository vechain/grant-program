# VeChain General Grant Application Template

## Project Overview 

- Project: WeFund from Terra Ecosystem
- Team Name: Andrea Bello, Ika Nur Affifah 
- Payment Address: USDT (ERC 20) payment address. We don't accept payments for the program in other currencies at this stage.

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

Please provide the following:
- A brief description of the project.
Community crowdfunding and incubation launchpad with a focus on real-world projects implementing blockchain in their existing model.
- An indication of why your team is interested in creating this project within the VeChain Ecosystem.
WeFund base the mission to use the blockchain for solve real world proble, have real world impact, social impact or enviroment impact.
VeChain have the mission and vision to solve and have real world impact so this is the main reason we like to apply to you
- If relevant, an indication of how you will integrate tools and features (e.g., Sync2/Connex, fee delegation protocols, MTT, etc) to enhance your project. 
We will build in decentralise way using smart contract for do all, we like to implement a MultiChain level with stablecoin paymento on top of it and a way to bridge web2 to web3 using fait to stable payment and email wallet login for not crypto user
### Project Details

We expect the teams to already have a solid idea about the project's expected final state.
Therefore, we ask the teams to submit (where relevant):
- Mockups/designs of any UI components
www.wefund.app
- API specifications of the core functionality
www.wefund.app
- An overview of the technology stack to be used
- Documentation of core components, protocols, architecture, etc. to be deployed
Smart contract Workflow

Instantiate
input parameter
Wefund contract
admin: String, //Owner wallet address
wefund: String, //wefund wallet address
anchor_market: String, //Anchor market contract address
aust_token: String,  //aUST cw20 contract contract
vesting_contract: String, //Vesting contract address

Vesting Contract
admin: String  //Wefund contract address

Staking contract
owner: String,  //Owner wallet address
start_time: Uint128,  //farming rewards start time
reward_token: String  //reward token address - WFD token address



Register Community
-input parameter
Wallet
-functions
Register the community members






Create Project


-input parameter
id: Uint128,  //If new, 0, If else, Stored project info
company: String,
title: String,
description: String,
ecosystem: String,
createddate: String,
saft: String,  //saft document
logo: String,
whitepaper: String,
website: String,
email: String,
creator_wallet: String,   //project creator wallet address
collected: Uint128,  //Amount to be collected
milestones: Vec<Milestone>,
teammembers: Vec<TeamMember>,
vesting: Vec<VestingParameter>,
token_addr: String,

country: String,
cofounder_name: String,
service_wefund: String, //equity
service_charity: String,
professional_link: String

-function
Initialize the project state  variables
If id = 0, New create and store, 
if id > 0, Modify the Project informations on Wefund contract
Register the project informations on Vesting contract
If id = 0, set Project status to ::Wefund_approve
If id != 0, Keep the Project status



WeFund approve

-input parameter
Project_id  //Stored the project id

-functions
Checking the message sender is the same as wefund.
Checking the Project status is ::Wefund_approve
Turn the Project status to ::Whitelist_open



Register Whitelist
-input parameters
Project_id //Stored the project id
Card_type: //The type of card the user has (Platinum, Gold, Silver, Bronze)

-functions
Checking the user is the card holder
Store the user wallet address and card type












Close Whitelist

-input parameters
Project_id // Stored the project id

-functions
Checking the message sender is the same as project creator
Calculate the Card Holder ticket and the Community Holder ticket
Making the whitelist with wallet address and allocation, based on ticket price
( Storing the registered Card holder wallet and Community Wallet, allocation)
Turn the project status to ::Fundraising




Reopen whitelist

-functions
Checking the message sender is the project creator
Calculate the amount to be collected and will collect
Whitelist clear
Turn the project status to ::Whitelist


Set fundraising stage

-functions
Checking the message sender is the project creator
Turn the fundraising stage to next

Back to Project
-input parameters
project_id: Uint128,
backer_wallet: String,
fundraising_stage: Uint128,
token_amount: Uint128,
otherchain: String,
otherchain_wallet: String,

-functions
Checking the message sender is registered on whitelist
Store the backer informations in the project information
Transfer 5% to Wefund wallet
Deposit 95% to Anchor Market and measure the aUST token amount and store.
Store the backer informations in the Vesting contract, also
Checking whether the backed amount has reached the collected amount, If reached, making the Milestone vote list(include the Wefund address to stop the milestone), 
If a vesting token address is registered, transfer the vesting tokens from project_creator wallet to vesting contract, and send message starting the vesting to the vesting contract , turn the project status to ::Milestone_Releasing


Milestone Vote

-functions
Checking the message sender is registered on Milestone vote list.
Store the vote status in project informations

Checking whether that all voted, 
If all voted, calculate the aUST token amount to withdraw from the Anchor market.
c: collected amount, a: measured aUST token amount for project
m: amount - milestone step amount, x: aUST token amount to withdraw

x = m / c * a

Withdraw from the Anchor market and measure the UST amount(u) withdrawn from the Anchor market.

If u>m, transfer m UST to the project creator, (u-m) UST is stored on the Wefund smart contract for profit distribution.
If u<m, transfer u UST to the project creator.

Turn the milestone step to next
If milestone done, turn the project status to ::Done

Project fail(There is no UI)
-function
Checking the message sender is the project creator
Calculate the remained the aUST token amount for project
Withdraw from the Anchor market and measure the UST amount to be withdrawn.
Calculate the percent and the UST amount to be returned back.
Return back the USt to the backer wallet.

Project Complete(There is no UI)
-function
Checking the message sender is the project creator
Calculate the remained the aUST token amount for project
Withdraw from the Anchor market and measure the UST amount to be withdrawn.
Calculate the percent and the UST amount to be returned back.
Return back the USt to the backer wallet.

Card Holders


Problems to solve

While creating project, add to input the community allocation, now is fixed as 20%
While turning to Releasing status, calculating the vesting token amount(Whether Based on the backed total vesting token amount or inputed Vesting parameters, now based on vesting parameters to be inputted in creating)
While creating, add the many validation checks such as token price per stage.
Calculate the vesting token amount based on token price per stage.(Now is fixed 0.06 at private, 0.09 at presale)
Improve the UI for backed
While joining to Whitelist, reject the community wallet
While back project on invest_step2, invest_step3, add to many validation check such as max amount, card holder, registered in Whitelist
Point number issues(to fix, use Decimal type)
- PoC/MVP or other relevant prior work or research on the topic
MVP is www.wefund.app
### Ecosystem Fit
Are there any other projects similar to yours? If so, how is your project different?
Launchpad is consider competitor but we have this difference
-Free incubation service, no fee
-Milestone funds release after backers approval for protect the investor and limited the risk
-Stablecoin payment
-Bridge web2 to web3
-Real world impact based
## Team 

### Team members

- Name of team leader
- Names of team members

### Team Website

- https://<your_domain>

### Team's experience

Please describe the team's relevant experience. If the project involves development work, then we'd appreciated it if you can single out a few interesting codes commits made by team members on their past projects. 

### Team Code Repos

- https://github.com/<your_repo_1>
- https://github.com/<your_repo_2>

### Team LinkedIn Profiles

- https://www.linkedin.com/<person_1>
- https://www.linkedin.com/<person_2>


Andrea Bello
Co-Founder & CEO
He is the person behind the development of the Fan$quad smart
contract that was deployed on Col-4 during the Hackathon organized
by Terraformlab. He has a wealth of experience in coding, with a
deep understanding of C, C++, Javascript, VBA, Java, Python, Rust
languages (to name a few). In 2018 he moved his focus into Solidity,
PHP, & HTML 5, to follow his vision of creating advanced web3.0 applications integrated
with the blockchain. His role is to ensure the delivery of the smart contracts, web app,
and technical infrastructure. A serial entrepreneur, he built a Natural Mosquito Solution
based in Bali, a hotel & restaurant (Ristorante-Bar Lanca) in Switzerland, and a smart-
home startup designed to reduce electricity consumption.
https://www.linkedin.com/in/bello-andrea-380572b4/

Ika Afifah 
Co-Founder & CMO
A dynamic individual who worked at Tencent as an Operation Specialist, in the partnership division. Before Tencent, she was Senior Partnership Manager at Bigo, a Senior Account Executive position at one of the digital marketing agencies under Jet Group, and Manager at Waves, helping founders raise $1.2M in pre-seed funding. She is one of the founding partners and driving forces behind the concept of WeFund.
https://www.linkedin.com/in/ika-nur-afifah/

Achuth Chandran
CFO
Experienced financial professional and consultant. HEC Paris alumnus. ACCA Affiliate. With experience at KPMG, Sancta Capital and Trilogy Enterprises, Achuth has vast experience in the different avenues of corporate and investment finance. He currently leads Octave Advisory, a blockchain consulting firm based out of Dubai with the goal to help promote and expand the technology.
https://www.linkedin.com/in/achuth-k-chandran-b17880102/

Austin Taylor 
CCO
Comes from a background in investment and corporate finance. After completing his education he worked as a Business Analyst for Harman International in Seattle, Washington USA building AI applications to identify high-risk sale transactions. After this, he transitioned to Investment Management for Pegasus Tech Ventures located in Jakarta, Indonesia managing investment deals in the Southeast Asia region.
https://www.linkedin.com/in/austintaylor19/



## Development Roadmap 

This section should break out the development roadmap into a number of milestones. Since the milestones will appear in the grant contract, it helps to describe the functionality we should expect, plus how we can check that such functionality exists in the product. Whenever milestones are delivered, we refer to the contract to ensure that everything has been delivered as expected.

Below we provide an <b>example roadmap</b>. For each milestone:

- Please indicate the milestone duration, workload in terms of full-time equivalent (FTE) and cost. 
For our stage the milestone is
stamrt contract integration and tech to your chain, 6 weeks 20k
Marketing and community grow on your chain, 8 weeks 10k

After the time for integration and be ready we will have a Fundrasing, 8 weeks, IDO 1 week, TGE 3 day
- Please be sure to include a specification of the software. The level of details must be high enough so that we are able to verify that the software meets the specification.

THe smart contract is convert the exist one in Rust to your technology
- Please note that we require documentation (e.g. tutorials, API specifications, architecture details) in each milestone. This ensures that the code can be widely used by the community.
- Please provide a test suite, comprising unit and integration tests, along with a guide on how to run these.
- Please commit to providing dockerfiles for the delivery of your project.


### Example Roadmap for a dApp Application

#### Overview

|  | Milestone 1 | Milestone 2 | Total |
| - | - |- | - |
| Estimated Duration | 30 d | 30 d | 60 d |
| Full-time equivalent (FTE) | 2 | 1 | 3 |
| Cost (up to $ 30,000) | $ 5,000 | $ 10,000 | $ 15,000|

#### Milestone 1 — Smart Contract & Backend

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | Apache 2.0 / MIT / Unlicense |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial that can interact with the deployed smart contracts and backend service. |
| 0c. | Testing Guide | The code will have proper unit-test coverage (e.g. 90%) to ensure functionality and robustness. In the guide, we will describe how to run these tests |
| 1 | Smart Contracts | We will develop smart contracts that will...  (Please list the functionality that will be coded for the contracts) |
| 2 | Backend | "We will create a backend service that will... (Please list the functionality that will be coded for the backend)" |

#### Milestone 2  —  Frontend

...

#### Community engagement

As part of the Program, we require that you produce and publish at least one article/tutorial (e.g., on Medium). It should explain your work done as part of the grant.

## Future Plans

Please include the team's long-term plans and intentions.
Becama a multichain layer 1 launchpad for projects with utility and real world imapct
## Additional Information 

Any additional information that you think is relevant to this application that hasn't already been included.

Possible additional information to include:
- What work has been done so far?
MVP done
- Are there any teams who have already contributed (financially) to the project?
before we get 300k in terra on the fundrasing , unlukly all is going
- Have you applied for other grants so far?
- Extra information
We are from Terra Ecosystem

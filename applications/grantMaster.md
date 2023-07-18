# grantMaster

## Project Overview 

- Project: grantMaster
- Team Name: Antier Solutions
- Payment Address: 0x2492237FA7698B8F3B35F2be4be3B1128439Ec8d (USDC)

### Overview

Please provide the following:
- The Grant Management Web Application is a comprehensive software solution designed to streamline and enhance the process of managing grants. It aims to provide the VeChain Ecosystem with a centralized platform to efficiently handle grant applications, evaluation, tracking, reporting, and overall administration. By reducing the number of clicks, the web application will enable better navigation of data, better UI, greater ease and effectiveness in the grant management process.

## Project Details

### Key Features:

- Organised relevant data.
- Github API integration to carry out relevant actions.

Technical Architecture

![Technial Architecture](https://github.com/lawmeskiviahs/vechain-grants-program/assets/60818312/1db67363-2205-4485-bc2b-a7d3f56260b9)

### Core Components:

#### Front-End:
1. UI:

- Login Page: ![login](https://github.com/lawmeskiviahs/vechain-grants-program/assets/60818312/25acfe0b-ada5-425a-b201-2e0afa4dfff7)

- Project List: ![projectList](https://github.com/lawmeskiviahs/vechain-grants-program/assets/60818312/8377178f-d2ed-4ad1-9000-474b9b7b80a8)

- Project Details: ![projectDetails](https://github.com/lawmeskiviahs/vechain-grants-program/assets/60818312/c41c9e73-b777-40b8-bab4-0308c219a167)

- Team Dashbard: ![teamList](https://github.com/lawmeskiviahs/vechain-grants-program/assets/60818312/fb737c81-0df2-421c-82dd-92620e5cfc5c)

- Team Details (applications): ![teamDetails](https://github.com/lawmeskiviahs/vechain-grants-program/assets/60818312/9f4f230d-8a93-4709-9b1d-a39d2bdfadc3)

- Team Details (projects): ![teamDetailsProject](https://github.com/lawmeskiviahs/vechain-grants-program/assets/60818312/afa48295-92d5-44cb-bff7-254fe7466253)


The discussions, commit, and file changes pages will be designed same as they are shown on a PR in github. Approvals, reviews and rejections will be handeled in the discussions tab

2. Back-End API Integrations

#### Back-End:

1. Front-End API Integrations
2. Github API Integrations
3. Database API Integration
4. Data Extractor - Service that extracts data from the MD files for storage
5. Web Hook Handler - Service that will listen to events and then handle the respective functionality

#### Database

- Schema: ![databaseSchema](https://github.com/lawmeskiviahs/vechain-grants-program/assets/60818312/bce482e2-0c87-4559-9173-9472f15cd3fd)

### Things not included in the project:

There is no in-app payment system in this application but these can be integrated upon further discussion.

### Technology Stack

- Front-end: HTML5, CSS3, JavaScript (React)
- Back-end: Node.js (Express.js)
- Database: MongoDB
- Authentication and Authorization: Github 
- Cloud Hosting: AWS

### Ecosystem Fit

- The VeChain grants program is growing by the day. It is quite a hassle for the committee to browse the Grant Program Repositories. This application aims to achieve two things: 1. Consolidate releveant information from the Grant Program Repos; 2. Provide Github Actions functionality to deal with the process of the Grant Program within the app itself.

## Team 

### Team members

- Rahul Saharan
- Jatin Sehgal
- Shaurya Awasthi

### Team Website

- https://www.antiersolutions.com/

### Team's experience

- Antier is a thought-to-finish partner for customers in their blockchain journey. We advise and consult our clients on blockchain technologies and tailor solutions utilising our powerful blockchain ecosystem. We help customers experiment and deploy proof-of-concepts on blockchain technologies and incrementally expand to scale to production releases. Our thought leaders regularly educate customers, partners, CXOs on the power of blockchain for today and tomorrow.
- Workdone by Antier in Substrate ecosystem
1. Antier worked on the validator and nominator apps for substrate based blockchains to offer a unique and better user experience .
2. We have also worked on creating an optimised and homogenised design focused on improving the navigation, information architecture, user flow tasks, content design and graphic elements for a seamless and easy browsing experience.
3. We have customised the default reward mechanism in the staking pallet of the substrate chain by integrating the sustainability and reliability score(which is calculated by ESG scores and Uptime of the validators repectively) of the validators in the current reward system.
4. We were able to run EVM and WASM machines natively in the substrate chain so that the chain will be able to support both EVM(Metamask, Remix, Web3.js, etc) and WASM(WebAssembly target, INK framework, etc) tooling. 

### Team Code Repos

- [Rahul Saharan](https://github.com/RahulS100)
- [Jatin Sehgal](https://github.com/JatinAntier)
- [Shaurya Awasthi](https://github.com/shauryaawasthi)

### Team LinkedIn Profiles

- [Rahul Saharan](https://www.linkedin.com/in/rahul-saharan-80035b186)
- [Jatin Sehgal](https://www.linkedin.com/in/jatin-sehgal-694b1776)
- [Shaurya Awasthi](https://www.linkedin.com/in/shaurya-awasthi)

## Development Roadmap 

### Roadmap for grantMaster

#### Overview

|  | Milestone 1 | Milestone 2 | Total |
| - | - |- | - |
| Estimated Duration | 30 d | 30 d | 60 d |
| Full-time equivalent (FTE) | 2 | 2 |  |
| Cost  | $ 12,500 | $ 12,500 | $ 25,000|

### Milestone 1  — Teams and Projects 

- **Estimated duration:** 4 weeks
- **FTE:**  3
- **Costs:** 12,500 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 |
| **0b.** | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can browse through the application and perform github actions |
| **0c.** | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| **0d.** | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 1. | Frontend | We will provide dashboard and details pages for Projects and Teams with all details |
| 2. | Backend | Database integrations and data extractor will be implemented. i.e data from the md files on github will be processed and saved to the database using API |
| 3. | Data Base | DB schema implementation |

### Milestone 2 Example — Applications and Deliveries

- **Estimated duration:** 4 weeks
- **FTE:**  3
- **Costs:** 12,500 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 |
| **0b.** | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can navigate through the data and perform github actions |
| **0c.** | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| **0d.** | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article**/workshop that explains [...] (what was done/achieved as part of the grant). (Content, language and medium should reflect your target audience described above.) |
| 1. | Frontend | We will provide dashboard and details page for the remaining tabs i.e Applications and Deliveries |
| 2. | Backend | Github API integrations and web hooks will be implemented so that our application can listen to events and make necessary changes in the db |

## Future Plans

In app payment system integration is being researched meanwhile and also looking for decentrallised alternative for github. Upon further discussions with the grants committee we shall go ahead with this

## Additional Information 

A minimal POC has been made wherein the basic github actions were successfully tested.
Things tested in POC:
1. Created issue in a repo
2. Fetch list of issues in a repo.
3. how to use responses.
4. Get PR list to a repo
5. Get PR by number
6. Merge a PR
7. Get comments on a PR
8. Update a comment on PR
9. Add comment on PR

- POC (code)- [ghApi](https://github.com/lawmeskiviahs/ghApi)
- POC (tested on) [helloGhpi](https://github.com/lawmeskiviahs/helloGhapi)
- [Github API Ref Sheet](https://docs.google.com/spreadsheets/d/1uzOTAQAgcDNR1n51U1KhnRKD-as1qP8UYBLDMNLm2t4/edit#gid=0)

Github provides REST API for a lot of github actions. The link to the API docs is [here](https://docs.github.com/en/rest?apiVersion=2022-11-28)

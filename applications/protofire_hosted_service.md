# VeChain General Grant Application Template

## Project Overview 

- Project: TheGraph Hosted Service
- Team Name: Protofire
- Payment Address: 0x63d6287D5b853cCfedbA1247fBEb9a40512F709A

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

To onboard developers, L1 networks must provide developers with a set of essential building blocks. We call these essential building blocks a “Minimum Viable Infrastructure.” Without offering essential services, the unique capabilities of Hedera are simply not available to consume. 

At Protofire, we specialize in removal of blockers that prevent organic growth of developer ecosystems. 

Imagine you are a developer who built a game or a novel DeFi application. You really like the throughput, time to finality and native file storage capabilities of VeChain. However, without standard querying of on-chain data you can’t utilize existing indexing/querying components and interfaces. You have to hire more engineers to deploy on VeChain vs deploying on another chain. 

This proposal brings The Graph protocol services, the #1 data indexing standard and its subgraphs, to VeChain. 

![image](https://user-images.githubusercontent.com/76965543/213206294-d9699fea-b758-4b15-987d-6c17221e8155.png)

Now, if you are a dApp developer, you can port existing dApps from other EVM chains without building your own data indexing/querying layer (unlike before, where you either stay away from deploying on Hedera or must hire additional developers/raise additional funding to deploy on Hedera vs other chains). 

As a result, a greater percentage of developers considering VeChain will reach deployment and production stage. 

After integration of The Graph, Protofire will be making separate proposals to bring industry leading oracles such as Chainlink, and multi-sig wallets such as Gnosis Safe to VeChain. 


### Project Details

The goal of this proposal is to:
- Provide a secure, timely & accurate service to the network users & Dapps.
- Have a scalable platform in a fast-growing ecosystem.
- Rely on a robust decentralized infrastructure and simultaneously access high-availability data service.
- Implement an infrastructure in the cloud based on the best practices. 

This proposal will provide the following services:
- Compatibility & pre-feasibility testing
- The Graph Cluster Implementation
- The Graph Cluster Maintenance
- Subgraph Development Service 

All of these services combined offer seamless integration into reliable infrastructure that will increase performance, security, and scalability.

From a Business perspective, this kind of infrastructure will embrace decentralization and, at the same time, will have a premium service that allows for a better analytic user experience and more adoption.

In the case of EVM-compatible networks with more throughput relying on a premium infrastructure is even more critical to generating adoption. This kind of service will not only make it easier for developers but also will allow dApps to offer a better experience to its users.

**Architecture**

In the next diagram we can use the same Erigon node in both environments if we want to reduce cost (3)

![image](https://user-images.githubusercontent.com/76965543/213208368-b1a06e24-d448-4f55-aafe-fd33d8b63e23.png)

**Architecture components** 

*Kubernetes*

Amazon Elastic Kubernetes Service (Amazon EKS) gives you the flexibility to start, run, and scale Kubernetes applications in the AWS cloud or on-premises. Amazon EKS helps you provide highly-available and secure clusters and automates key tasks such as patching, node provisioning, and updates.

*Terraform*

Terraform is an open-source infrastructure as code software tool that provides a consistent CLI workflow to manage hundreds of cloud services. Terraform codifies cloud APIs into declarative configuration files.
We use Terraform to automate all services and deploy them on AWS. This allows us to maintain a control version of the infrastructure and also to keep the security rules under supervision.


## Team 

### Team members

- Team Leader: Diego Torres
- Team members: - Braian Leiva
                - Ramiro Vazquez 
                - Luis Lopez 


### Team Website

- https://protofire.io/

### Team's experience

Protofire is one of the oldest and biggest indexers on The Graph Network. We accrued a great deal of experience working with this infrastructure that can help other protocols to join the network or enjoy its functionality. 

### Team Code Repos

- https://github.com/<your_repo_1>
- https://github.com/<your_repo_2>

### Team LinkedIn Profiles

- Braian Leiva - DevOps - https://www.linkedin.com/in/braian-leiva/
- Ramiro Vazquez - Full Stack Dev - https://www.linkedin.com/in/ramirotw/
- Luis Lopez - Subgraph Developer - https://www.linkedin.com/in/luigibyte/ 
- Diego Torres - Project Manager - https://ar.linkedin.com/in/diego-torres-borda-94b70912/


## Development Roadmap 

![image](https://user-images.githubusercontent.com/76965543/213213810-fdcd1751-6530-4cbf-8b80-42842681e906.png)


Maintenance plan can be recalibrated after 3 months. 

*Deliverables:*

The Graph Cluster Infrastructure
Github script to create infrastructure
UI for User to see subgraph and access to the endpoints
Developer Tutorial: How to deploy subgraphs
Monitoring & Subgraph error logging 



## Infrastructure costs

![image](https://user-images.githubusercontent.com/76965543/213214669-a6fc979f-8897-4bff-a701-d2cf3ddda221.png)

![image](https://user-images.githubusercontent.com/76965543/213214719-66d99a83-c89d-48fe-9512-b3051a0581d5.png)

![image](https://user-images.githubusercontent.com/76965543/213214794-f068f741-d7ba-4255-b331-6ea0dccf276b.png)

(1)  536.396 GB processed
(2)  2,772.219 LCU-Hrs - 1,222.000 Hrs
(3) We can avoid Erigon mainnet in the dev environment if we want to reduce cost. See diagram above.


## Assumptions

1) Estimate is approximate and may vary depending on further requirement changes, clarifications or uncovered complexities. 
2) VeChain team is going to provide Protofire team with access to an AWS account that has enough access level to deploy all the required components (e.g. RDS, EC2, ECS/EKS, etc.).
3) The infrastructure cost might be around 10% higher than calculated due to additional payments like data traffic, monitoring, etc. 
4) The infrastructure cost might differ depending on the usage volume
5) The infrastructure cost might increase if VeChain agrees to send the infrastructure logs to OpenSearch service.


# VeChain General Grant Application Template

## Project Overview 

- Project: Tali AI
- Team Name: Tali AI LLC
- Payment Address: 0xc5F1C802F56e34B05e9aAfBFE0302c6595405035

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

Please provide the following:
- **A brief description of the project.**

We propose to develop a private bot or a widget for VeChain, leveraging the power of advanced Large Language Models (LLMs). This tool would integrate various resources such as VeChain's Github repositories, documentation, associated articles, and Q&A history, creating an interface where users can ask questions in a natural language. The primary objective is to enhance Developer Relations, Customer Support, and Community Support within the VeChain ecosystem. This solution would streamline the support process and expedite responses to frequently asked questions, fostering a better user experience and more effective utilization of support resources.

- **An indication of why your team is interested in creating this project within the VeChain Ecosystem.**

Our team recognizes the increasing importance of blockchain technology and the pivotal role VeChain plays in this domain, specifically with its public blockchain platform focused on supply chain management, smart contracts, and secure data management. We believe that enhancing developer and community support for VeChain will play a significant role in broadening its adoption and fostering a more vibrant ecosystem.

VeChain's expansive documentation and active community present an ideal environment for our proposed project. With its unique focus on both business applications and individual users, the VeChain platform presents a challenging and exciting opportunity for us to create a tool that can significantly benefit both these sectors.

Our team, led by Ali Agha and Tenzin Rose, has considerable experience in decentralized solutions and delivering quality technical solutions. This project aligns with our expertise and our vision of advancing blockchain technology. We are committed to creating a more equitable world through the power of decentralization, and we see VeChain as an essential component of that vision.

- **If relevant, an indication of how you will integrate tools and features (e.g., Sync2/Connex, fee delegation protocols, MTT, etc) to enhance your project. **

Given this is a developer / community support bot our stack will implement ML tools (listed below). 

### Project Details

We expect the teams to already have a solid idea about the project's expected final state.
Therefore, we ask the teams to submit (where relevant):

**Technology stack**
- OpenAI 
- Llama Index
- Digital Ocean (hosting)
- Deeplake (Vector DB)
- Supabase 
- Cohere

**Workflow of question / answer**
![image](https://github.com/niznet89/grant-program/assets/81620032/6311b9bf-be2c-4af2-a60d-8adce2559d16)

**MVP**

We have a working MVP of Tali which we can invite VeChain team members in to test. 

### Ecosystem Fit
Are there any other projects similar to yours? If so, how is your project different?

Yes, there are indeed other projects that seek to use AI and Large Language Models (LLMs) to streamline customer and developer support, given the high demand for such solutions in the tech industry. However, our project, "Tali," stands apart in a number of ways:

1. VeChain Focused: Tali is specifically designed for the VeChain ecosystem. This means our project is not just a generic support tool, but one that is carefully tailored to the unique features, questions, and community behaviors associated with VeChain. This level of specialization can lead to a more accurate, effective, and user-friendly support experience.

2. Continuous Learning and Adaptation: Tali is planned to be a continuously evolving tool. It is not just about deploying an AI, but about constantly optimizing it based on feedback and new data. This approach ensures that Tali will continually improve and adapt to changing user needs and technological advancements.

3. Community Collaboration: From the very start, Tali is being designed with a community-focused approach. We plan to work closely with VeChain's DevRel, Customer Support, and Community Support teams to ensure that Tali addresses their most pressing pain points and integrates seamlessly into the existing ecosystem.

## Team 

Ali Agha is a technologist and entrepreneur focused on decentralized solutions. In his previous venture, Olypsis Technologies, Ali offered Web3 consulting services to countless startups and big corporations like IBM and Thomson Reuters. Ali started his journey in the blockchain space in 2015 when he discovered bitcoin. Since then, he has dedicated his career to creating a fairer and more equitable world through the power of decentralization.

Github: https://github.com/OlypsisAli 
Twitter: https://twitter.com/iamAliAgha

Tenzin Rose is an entrepreneur and full-stack developer with a background in enterprise sales. He's worked with global startups and enterprises, helping them successfully deploy projects and generate revenue. His current interests lie in web development and deciphering the complex equations in ZKP and ML.

Github: https://github.com/niznet89
Twitter: https://twitter.com/tenzin_rose

### Team Website

- https://trytali.com

### Team's experience

Please describe the team's relevant experience. If the project involves development work, then we'd appreciated it if you can single out a few interesting codes commits made by team members on their past projects. 

Tenzin personal project: https://github.com/niznet89/nomad-map
Ali hackathon project: https://github.com/OlypsisAli/portal

### Team Code Repos

- [Ali Agha Github](https://github.com/OlypsisAli)
- [Tenzin Rose Github](https://github.com/niznet89)

### Team LinkedIn Profiles

- [Ali Agha Linkedin](https://www.linkedin.com/in/ali-agha/)
- [Tenzin Rose Linkedin](https://www.linkedin.com/in/tenzinrose/)

## Development Roadmap 

### Development Roadmap for Tali Bot/Widget

#### Overview

|                   | Milestone 1 | Milestone 2 | Total  |
|-------------------|-------------|-------------|--------|
| Estimated Duration| 2 weeks     | 2 weeks     | 4 weeks|
| Full-time equivalent (FTE) | 1.5  | 1.5  | 3 |
| Cost (up to $ 7,500)| $3,750     | $3,750     | $7,500 |

#### Milestone 1 — Implementation of Data Sources

| Number | Deliverable | Specification |
|--------|-------------|---------------|
| 0a.    | Documentation | We will provide a basic tutorial on how to interact with the bot/widget using different data sources. |
| 1      | Data Source Integration | We will integrate 3-4 high-value data sources into the bot/widget. This will include VeChain's Github repositories, documentation, related articles, and Q&A history. |
| 2      | Index Creation | We will use the Llama Index to create indices and a vector database to facilitate embeddings-based search on queries. |
| 3.     | Deployment to private Discord server where members of the VeChain team & community can test out Tali. The team will be asked to up / down vote responses for future training |

#### Milestone 2  —  Testing, Optimization, and Deployment

| Number | Deliverable | Specification |
|--------|-------------|---------------|
| 0b.    | Documentation | We will update the existing documentation to cover new features and optimizations. |
| 1      | Bot/Widget Testing and Optimization | We will focus on eliminating any hallucinations and refining the bot's/widget's prompt engineering to ensure it gives only relevant answers. |
| 2      | Deployment | The bot/widget will be production-ready and approved by the Customer / Community Support teams. It will be ready for deployment on VeChain's support channels. |
| 3      | Bot learning | Based on team / community responses from initial deployment, custom data will be provided to Tali to help answer future questions. |


#### Community engagement

We understand the importance of community engagement and outreach. We commit to producing and publishing at least one article or tutorial on Medium, detailing the progress and achievements of our project as part of the grant. This article will aim to help users understand the value and usage of the Tali Bot/Widget in the VeChain ecosystem.

We are also prepared to engage in Discord discussions and participate in community events to drive the adoption of our tool and assist users in the best possible way. Our goal is to ensure the VeChain community feels supported and heard throughout the development and deployment of the Tali Bot/Widget.

## Future Plans

Our team envisions the Tali Bot/Widget as a multi-faceted tool that grows with the needs of the VeChain community and continues to be a key resource for developers, customers, and the broader community.

**Long-Term Project Plans:**

React & Vanilla JS Widget: We plan to develop a widget using React and Vanilla JS, providing a component that can be easily added to the VeChain documentation page. This widget will be interactive, allowing users to ask questions directly on the docs page and receive instant responses, thus enhancing the accessibility and usability of our tool.

Analytics Suite: We recognize the value of data-driven insights in shaping a project's growth. We intend to implement an analytics suite that will track the types of questions the community is asking, enabling us to continuously improve the bot's responses and understand the community's needs better.

Knowledge Graphs: We plan to delve deeper into the understanding of the VeChain codebases by creating knowledge graphs. These graphs will help the bot understand complex queries better, leading to more accurate and contextually aware responses.

**Operation Plans:**

We are committed to regular maintenance and updates to keep the bot's knowledge up-to-date and its performance optimal. We will periodically engage with the VeChain community, gather feedback, and iterate on the bot's features and functionalities. This includes refining our algorithms, updating our data sources, and enhancing our user interface based on user feedback and needs.

**Intention:**

Our overarching intention is to create a product-driven solution where customers can self-serve effectively and efficiently. We want Tali to be a robust and reliable tool for all users, from novice developers to experienced ones, to community members who are interested in VeChain's growth and development. Additionally, we recognize that some users might require custom implementations to better suit their needs.


## Additional Information 

Any additional information that you think is relevant to this application that hasn't already been included.

Possible additional information to include:
- What work has been done so far?

We have a working MVP of the product. 

- Are there any teams who have already contributed (financially) to the project?

We have recieved other grants (see below). 

- Have you applied for other grants so far?

Yes: Solana Foundation, Lens Protocol, and Balancer. 

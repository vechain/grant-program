# VeChain General Grant Application Template

## Project Overview 

- Project: Awesome VeChain
- Team Name: Tolga Yaycı (Individual)
- Payment Address: [0xa632439DE1592936fbA3368053eaafd491443493](https://etherscan.io/address/0xa632439DE1592936fbA3368053eaafd491443493) (USDC, Ethereum (ERC20))

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

Awesome VeChain - the ultimate social platform for discovering and exploring the most exciting projects in the VeChain ecosystem! Whether you're a developer, investor, or simply a curious enthusiast, Awesome VeChain provides a one-stop-shop for accessing comprehensive and detailed applications about the projects. With this cutting-edge platform, you can discover the latest updates and developments, connect with project owners, and stay up-to-date with the most innovative projects in the VeChain community.

### Project Details

The project consists of three main parts: a public frontend, a dashboard where project owners can update the projects, and an admin dashboard where admins can perform some operations on the projects.

Aws Dynamo Db and Aws Appsync (graphql) are used together for the project backend, new users and projects are added to the database using the GraphQl API with the relevant operations. Meanwhile, auth transactions are managed with the AWS Lambda service. For example, when a project enters its account using its wallet, a token is generated with the Lens API, and on the server side, it is checked from which address the token produced by this relevant wallet was produced and whether it is valid. If it is valid, it can continue its functions as much as allowed.

Algolia is used as the search infrastructure, and thus, users can quickly perform detailed global searches on the page and expand their search scope by using the filters they want on the project page.

Technology Stack:

- AWS App Sync (GraphQL)
- AWS Amplify
- Next.js
- Redux
- Tailwind CSS
- Wallet Connect, Lens API (Web3 Auth & Wallet)
- Algolia (Search Infrastructure) 

---------

**Public Page**

- Home Page: Visually appealing and user-friendly homepage which includes latest articles, popular categories and many more
- Projects Page: Showcase page with detailed filtering and search infrastructure
- Project Detail Page: Project details page to display detailed information about project with several modules 
- Articles Page: Articles page to showcase informative articles related to the subject
- Article Detail Page: Detail page for individual articles to display their full content
- Ranking Page: Ranking page based on votes and token stats which is supported by CoinGecko api to showcase popular projects and articles
- Learn Page: Useful resources to learn about VeChain ecosystem


**Project Owner Dashboard** 

- Main Page: Homepage that displays statistics about the project
- Project Page: Management page for project detail page with 6 modules like description, token stats and so on
- Articles Page: A page that has give ability to update or write articles with built-in editor
- Profile Page: Displays to core areas about project and gives ability to update

**Admin Dashboard** 

- Main Page: Homepage that displays statistics about the Awesome VeChain
- Projects Page: A page which gives rights to admins approve, reject or change status of projects
- Roles Page: This page will provide the ability to update project owner and admin roles.

### Ecosystem Fit

No, I could not find such a project listing platform in the vechain ecosystem.

## Team 

### Team members

- Tolga Yaycı

### Team Website

- [GitHub](https://github.com/tolgayayci/)

### Team's experience

As a full-stack developer with 2 years of experience, I have honed my skills in software development, with a focus on dApp development in the past year. I have a deep interest in the Web3 and NFT space and have put my skills to the test by creating a number of relevant applications. In addition to my experience, I have developed detailed React and Next.js projects, further enhancing my ability to build robust and scalable web applications.

In addition to my technical skills, I have also been actively involved in the wider tech community. I have served as a Chainlink Community Advocate, Aave Turkey Community Manager, and Founding Chair of Gazi University ACM Student Chapter. My previous role as a Microsoft Learn Student Ambassador has also given me the opportunity to share my knowledge and experience with others. I have set of experiences and skills and particularly in the areas of full stack software development and community management.

I have a track record of successfully developing and completing applications for various protocols, including Aave, Polkadot, Lens Protocol, Filecoin, and others.

### Team Code Repos

- https://github.com/tolgayayci

### Team LinkedIn Profiles

- [LinkedIn](https://www.linkedin.com/in/tolgayayci/)

## Development Roadmap 

Roadmap is defined a one milestone. This is a kind of integration grant application and detailed will be explained in the following sections.

#### Overview

|  | Milestone 1 | Total |
| - | - |- |
| Estimated Duration | 30 d | 30 d | 
| Full-time equivalent (FTE) | 1 | 1 |
| Cost (up to $ 30,000) | $ 5,000 | $ 5,000 | 

#### Milestone 1 - Integration

- **Estimated duration:** 1 month
- **FTE:**  1
- **Costs:** 5,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a**.| License | MIT |
| **0b.** | Documentation | I will provide both inline documentation of the code and a basic tutorial that can overview the platform.|
| **0c.** | Testing Guide | The code will have proper unit-test coverage (e.g. 90%) to ensure functionality and robustness. In the guide, we will describe how to run these tests |
| **1.** | UI & UX Development | **Home Page:** Visually appealing and user-friendly homepage which includes latest articles, popular categories and many more <br /><br /> **Projects Page:** Showcase page with detailed filtering and search infrastructure </br></br>**Project Detail Page:** Project details page to display detailed information about project with several modules like explained in the solution <br /></br>**Articles Page:** Articles page to showcase informative articles related to the subject <br /></br>**Article Detail Page:** Detail page for individual articles to display their full content <br /></br>**Ranking Page:** Ranking page based on votes and token stats which is supported by CoinGecko api to showcase popular projects and articles </br></br> **Learn Page:** Useful resources to learn about VeChain ecosystem </br></br> **UX Improvements & Testing:** I will work to improve the user experience by ensuring that the user interface is fully compatible with mobile and tablet devices. |
| *2.* | Project Owner Dashboard  | As part of this milestone, I will be implementing both the frontend and backend components of the Project Owner Dashboard. This involves designing and developing the user interface (UI) for the dashboard, as well as building the necessary backend infrastructure to support its functionality. To ensure the quality of my work, I will conduct thorough testing to ensure that the dashboard is user-friendly and performs as expected. My ultimate goal is to provide project owners with a seamless and efficient experience when updating their pages and publishing articles on our platform.

#### Community engagement

I will provide necessary articles and links after the project completed. I will also share the project on my social media accounts and will try to get feedback from the community.

## Future Plans

- I will publish a forum post on that will introduce Awesome VeChain and solicit feedback from the communityI will gather feature requests through a dedicated webpage
- After reviewing the feedback and votes, I will determine which new features to prioritize
- In addition to the forum, I will also collect feedback through social media channels such as Discord and Twitter
- I will establish contact with at least 30 project owners who are building on VeChain and add their projects to the Awesome VeChain
- I will manage the **@awesomevechain** Twitter account and keep the followers of the Awesome VeChain community updated on the latest projects added to the platform. Monthly threads will be created to share developments with the community.
- I will seek to establish partnerships with DAOs and domain allocators in order to make our platform more sustainable.
- I will collect analytics on user engagement to inform further improvements.

## Additional Information 

Several protocols are currently actively using the awesome series and have provided grants.

Lens Protocol: https://dev.awesomelens.xyz

Project is mostly developed and ready to ship for VeChain program, if there will be another feature requests I am eager to implement that to platform. 

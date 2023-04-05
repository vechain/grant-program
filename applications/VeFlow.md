# VeFlow Grant Application

## Project Overview 

- Project: VeFlow
- Team Name: justmert 
- Payment Address: 0xf5412558d977915D56d8B4d3773871142d379E74

### Overview

As the VeChain protocol ecosystem continues to grow, it's becoming increasingly challenging to stay informed about the ecosystem's status and trends, as well as the activities of the many open-source projects being built on or integrated with the protocol. With data scattered across various platforms through Github to Twitter, gaining a comprehensive view of the ecosystem can be a daunting task.

VeFlow offers a cutting-edge solution to this problem, providing a comprehensive platform that delivers various insights and metrics to track the activities and development of the VeChain ecosystem. Through intuitive and interactive visualizations and charts, VeFlow empowers users to gain a clear understanding of code contributions, community engagements, trend data, and many other critical metrics related to the VeChain ecosystem.

By tracking various off-chain sources, VeFlow is the go-to platform for gaining a comprehensive view of the VeChain and becomes uniqueness in the space.

### Links

* MVP Website: <https://veflow.netlify.app/>
* Open-source Backend: <https://github.com/justmert/eco-pulse-backend>
* Open-source Frontend: <https://github.com/justmert/eco-pulse-frontend>

### Project Details

#### Website 

| Dashboard Page | Project List Page | Project Page |
| --- | --- | --- |
|![Screenshot 2023-04-05 at 17-07-32 VeFlow](https://user-images.githubusercontent.com/37740842/230108020-cff33e1f-66d6-4a9c-968e-a8833bfeac69.png)|![Screenshot 2023-04-05 at 17-17-22 Projects](https://user-images.githubusercontent.com/37740842/230109171-3141145a-f7c8-4a6b-9b7a-6cb3fb7d1fe9.png)| ![Screenshot 2023-04-05 at 17-12-46 Project Page](https://user-images.githubusercontent.com/37740842/230108140-37d4f2c5-3bca-4ee9-9b5f-e49e4cdcebc4.png)|


#### Technical Scheme
![fvmflow_technical_scheme (4) (1)](https://user-images.githubusercontent.com/37740842/230104096-97a1db91-77de-44ae-af44-ca33a06537a0.png)


### Ecosystem Fit

* **Comprehensive analytics platform:** VeFlow provides a comprehensive platform that delivers various insights and metrics to track the activities and development of the VeChain ecosystem and its associated open-source projects.

* **Consolidated data sources:** By consolidating data sources and presenting key metrics and insights in an intuitive and interactive format, VeFlow addresses the challenge of scattered data sources, making it easier for users to understand the ecosystem's status and trends.

* **Helping to make informed decisions:** By providing valuable insights and metrics, VeFlow can help ecosystem users make more informed decisions about which projects to support and contribute to as well as identify promising projects and high-risk ones.

* **Gap in the market:** VeFlow fills the gap in the market by being the only project that becomes go-to core off-chain analytics dashboard for the VeChain ecosystem.

* **Discovering the evolution of the ecosystem:** VeFlow provides historical data and visualizations of key metrics, enabling developers and ecosystem users to better understand the development trajectory of VeChain and its projects. This feature helps users identify areas where protocol gains trends and track the ecosystem's progress over time.

* **Integration with approved grants and hackathons:** VeFlow can be integrated with approved grants and hackathons to keep track of the activity and development of these projects within the VeChain ecosystem. By tracking the progress and development of grant recipients and hackathon projects, VeFlow can provide valuable data and visualizations, which can be used to evaluate the success of these programs and their impact on the ecosystem.

* **Encourage Community Collaboration:** VeFlow provides a centralized location for viewing project activity and contributions, encouraging community collaboration and engagement. By enabling users to easily identify areas where they can contribute to projects, thus empowers the community to work together towards a common goal, further strengthening the VeChain ecosystem.


## Team 

### Team members

- Mert Köklü

As an experienced Web3 developer, I have become a grantee for Web3 Foundation, AAVE, Lens and Filecoin ecosystems by developing innovative projects. As a certified NVIDIA instructor, AAVE Turkey Community Co-Manager and ambassador for organizations such as Microsoft and The Graph protocol, I have become a trusted voice within the communities and gained a deep understanding of their needs and requirements. 

Currently, I'm focused on developing open-source and user-friendly applications that bring value to the VeChain ecosystem.


### Team Website

- Github: https://github.com/justmert
- Stack Overflow: https://stackoverflow.com/users/10515117/mert-köklü

### Team Code Repos

- [AaveQL](https://www.aaveql.org/): Aave GraphQL Documentation (Received grant from Aave) 
- [Peer-CLI](https://github.com/justmert/peer-cli): Swiss Army Knife for the IPFS (Received grant from Filecoin)
- [Aave API Telegram Bot](https://github.com/justmert/Aave-API-Telegram-Bot): Aave GraphQL Documentation (Received grant from Aave)
- [chainweb.py](https://github.com/justmert/chainweb.py): Kadena Chainweb Python Bindings

### Team LinkedIn Profiles

- https://www.linkedin.com/in/mertkoklu/


## Development Roadmap 

### Overview

|  | Milestone 1 | Milestone 2 | Total |
| - | - |- | - |
| Estimated Duration | 30 d | 45 d | 75 d |
| Full-time equivalent (FTE) | 1 | 1.5 | 2.5 |
| Cost | $ 8,000 | $ 9,500 | $ 17,500|

### Milestone 1

* Budget: $8,000
* Estimated Time: 1 month

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | MIT |
| 0b. | Documentation | I will provide both **inline documentation** of the code and a basic **how-to page** that explains how the user can interact with the platform |
| 1. |  Database | Set up a Firebase project and Firestore database to store chart data and project metadata. |
| 2. |  Backend | To integrate Github Data to the VeFlow, develop a Python backend that uses both the Github Rest and GraphQL APIs to fetch latest data from the Github. |
| 3. |  Frontend | Build the Project Detail and Dashboard pages, including the following implementations: Commit History By Weeks, Code Frequency, Top Contributors, Issue Activity, Issue Count, Star Count, Pull Request Count, Recent Issues, Recent Commits, Pull Request Activity, Recent Stargazing Activity. |
| 4. |  Frontend | Build a Project List page that lists all VeChain ecosystem projects in order of their respective stargazing counts. |
| 5. |  Integration | Integrate Algolia to improve the search functionality of the platform. |
| 6. |  Integration | Integrate Typeform to allow ecosystem users to suggest new projects for the platform. |
| 7. |  Integration | Integrate Google Analytics to track user engagement and improve the platform accordingly. |
| 8. |  Backend | Set up a regular update schedule for the backend to keep the database up-to-date with the latest data. |

### Milestone 2 

* Budget: $9,500
* Estimated Time: 1.5 month

| Number | Deliverable | Specification |
| --- | --- | --- |
| 1. |  Feature | Integrate Twitter data of VeChain and its associated projects into the platform, including metrics such as the number of tweets posted per day or week, the number of likes, retweets, and replies received, and other relevant analytics. |
| 2. |  Feature | Develop categorization feature to classify projects based on various criteria within the VeFlow, such as DeFi, DEX. The feature will make it easier for users to find projects that are of interest to them. |
| 3. |  Feature | Develop project health score feature that evaluates multiple metrics to provide users with an overview of a project's health. The score helps identify promising projects and high-risk ones. The resulting score, weighted by metric importance, will display on the project detail page. |
| 4. |  Feature | Develop an API for VeFlow that provides developers with access to VeFlow charts and metadata. The API will use RESTful architecture and documented using OpenAPI Specification. Using the API, developers can embed charts and data into their own applications. |
| 5. |  Feature | Up-to-date ecosystem project list on VeFlow will be customized based on the protocol's preference. If the protocol wishes project list to be updated independently, a GitHub crawler will be implemented to automatically discover ecosystem projects and adds them to the VeFlow. Alternatively, if the protocol has a project list available on a platform such as Notion, we will use the platform's respective API to access the list. In addition, if the protocol has a website that displays its ecosystem projects, such as an awesome list or other third-party application, we can parse the GitHub links and incorporate them into VeFlow. We will collaborate with the protocol to determine the most effective approach and ensure the project list is kept up-to-date and accurate. |



## Future Plans

In the short term, we intend to use VeFlow to provide a comprehensive and user-friendly platform for developers and ecosystem users to track and analyze projects in the VeChain ecosystem. We will continuously enhance and update the platform to ensure that it is the go-to resource for up-to-date information on VeChain ecosystem. This includes adding new features as described in the second milestone.

In the long term, our team's plan is to continue supporting and improving VeFlow to meet the evolving needs of the VeChain community. This includes incorporating additional metrics and data sources to provide more detailed insights into projects. Besides, if the platform is well-received by the community, and gains traction, we are going to open a Twitter account for VeFlow to engage with the community and promote top open-source projects, and contributors on the VeChain ecosystem. 


## Additional Information 

Deployed frontend has initially small number of repositories because of the demo purposes. After the approval, VeFlow will have more repositories according to the mechanism to be decided with protocol as described in milestone 2. 

If you have any questions or requests, please feel free to contact me. We can schedule an interview so that I can explain the project in detail. Thank you.

* Email: kklumert@gmail.com
* Telegram: @mertkklu
* Discord: MertK#2634

# VeChain General Grant Application

## Project Overview 

- Project: Football guessing game
- Team Name: SayNode Operations AG
- Payment Address: 0x989A38EDEbd2Bd80d4949a9F7462C93FA8055876


### Overview
This is a guessing game for the upcoming football World Championship 2022. The guessing game will be based on VeChain and as global as possible. Of course, possible legal issues will be clarified for each juristiction.
The whole game will run on VeChain and a payment with VET in different pots will be possible (see further clarification below). We want to create the basis or proof-of-concept for other tournaments such as the European Championship but also build a solution that can be further expanded. For example, for UFC or E-Sports area and even include NFTs. 

### Project Details
 
The individual sub-steps and milestones are described in more detail below in the chapter Development Roadmap.

The project includes a guessing game for the World Cup 2022, where you can guess the result of the individual games with Crypto and win a prize at the end of the tournament. 
To make the guessing game open to different areas of the world, we would like to offer different "pots" (e.g. 5 USD, 10 USD, 100 USD). This is done to give as many people as possible the opportunity to participate in the guessing game. The focus is on the countries participating in the World Cup. 

For this purpose, a website is created through which a user can connect to his wallet. The user then has the options of the individual pots which he can participate in. It is up to the user whether he wants to play in only one pot or in several pots, but in each pot he/she can play only once per address. When the user has decided and entered a pot, the values are stored in a smart contract. Now the user has the possibility to guess on the different games of the group phase. He can guess the outcome of the game until 23.59 CET of the previous day, but he is free to guess the results of all known games. As soon as the group stage is over, you can continue on the round of 16, then the quarterfinals and so on. The exact dates are defined below. Since there was already a postponement of the first game as well as one in the last European Championship, the contracts will be upgradable.

After each game, the points are awarded to the players according to the definition below. A leader board will be created where each player can see their current rank. This ranking will be adjusted after each game. At the end of the tournament, the pots are automatically paid out by the Smart Contract to the corresponding winning addresses. 

In addition to the website for the guessing game, we will also create an app with Flutter that is available in both the Appstore and the Google Play Store in order to reach as many customers as possible. The app can also be used to guess on the various games. 

Matches
 ----> Group games 48 matches / start on 20.11.2022

 ----> Round of 16, 8 matches / start on 3.12.2022

 ----> Quarterfinals 4 matches / start on 9.12.2022

 ----> Semifinals 2 matches / start on 13.12.12.2022

 ----> Match for third place 1 match / start on 17.12.2022

 ----> Final 1 match / start on 18.12.2022

 ----> Total 64 games 

 Point distribution

 ----> Winner 20 (20 points / 2.5%)

 ----> Group matches: 5 points for the correct winner, 1 point per correct number of goals per team (2 in total), 3 points for the correct goal difference / 10 points possible per match (Total: 480 points / 58%)

 ----> Round of 16 matches: 10 points for the correct winner, 2 points per correct number of goals per team (4 in total), 6 points for the correct goal difference / 20 points possible per match (Total: 160 points / 19%)

 ----> Quarterfinals: 10 points for the correct winner, 2 points per correct number of goals per team (4 in total), 6 points for the correct goal difference / 20 points possible per match (Total: 80 points / 9.5%)

 ----> Semi-final matches: 10 points for the correct winner, 2 points per correct number of goals per team (4 in total), 6 points for the correct goal difference / 20 points possible per match (Total: 40 points / 4.9%)

 ----> Match for third place: 10 points for the correct winner, 2 points per correct number of goals per team (4 in total), 6 points for the correct goal difference / 20 points possible per match (Total: 20 points / 2.5%)

 ----> Final: 15 points for the correct winner, 3 points per correct number of goals per team (6 in total), 9 points for the correct goal difference / 30 points possible per match (Total: 30 points / 3.6%)

 Total: 64 matches / 830 points 

 With this point distribution we allow that people who are experts in soccer have a higher chance to win. However, with smaller variables like choosing the winner at the beginning of the tournament, we allow an uncertain variable that brings in a bit more luck and a chance for unexperienced players. By steadily increasing the points from the group stages to the final, the excitement is maintained throughout the tournament. With the total number of points of 830 over 64 matches, we also want to avoid having "many" players with the same number of points. 

Pots

Two to a maximum of three pots are created for the guessing game. A person can play once per pot per address.  
For the pots the current value is shown on the website as well as the sum of the payout. A percentage of each pot will go to SayNode (we expect around 5 percent). 

Payment

The payout will be sent to the different addresses via smart contract directly after the final. 
The amounts depend on how many players are playing and what the total amount is. 
If there are players who have the same number of points, they will take the following ranks and their winning amount. For example, if two players are in second place, the sum of second and third place will be added together and divided by two. 

![Home screen](https://saynode.ch/wp-content/uploads/2022/08/soccer.png)

### Ecosystem Fit

Our game allows the VeChain and broader crypto community a fun way to directly interact with smart contracts and use the immutable nature of the blockchain during an ongoing worldwide event. With the UFC advertising contract, VeChain has addressed a customer demographic that we can also leverage here. Likewise, at a later date, the product can be expanded to possibly become relevant to the UFC customer segments as well. This way we can show VeChain to new customer groups and create more awareness, as this is also our preferred Layer 1 solution.

## Team 

### Team members

- Renato Schär
- Werner Liechti
- Yann Marti
- Paula Amstutz
- João Morais
- Riccardo Mazzucchelli
- Francesco Romeo
- Simon Heer
- Ruthusanth Vijayakumar


### Team Website

- https://saynode.ch/

### Team's experience

The SayNode Operations team has already implemented several projects for the company, including for Vechain. Besides the token migration of Dohrnii Foundation https://dohrnii.io/ from Ethereum to Vechain, a first project directly for Vechain has already been implemented. Further, a grant has already been awarded by VeChain for the Dev-Thorkit-Dart see here: https://github.com/vechain/grant-program/pull/51, the implementation of the project is still ongoing. Besides, a first Flutter App was developed, which was accepted by the Apple Store as well as the Android Store and can be found here: https://github.com/SayNode/342. Overall, the team has experience with DAO creation, Wallet creation, Token and Multichain Tokens as well as ICOs.

Renato Schär and Werner Liechti were the CTOs of Dohrnii Foundation and are the CEO and COO of SayNode Operations. The Dohrnii project is a DAO solution with a native token DHN on Ethereum, VeChain and Binance Smart Chain. The technical implementation of the Dohrnii project is mainly done by SayNode Operations (https://dohrnii.io/). Both have a computer science background and a degree from a Swiss university. 

Yann Marti is a Flutter Developer at SayNode Operations. He is an absolute specialist and does all frontend work for the Vidaia app as well as for Dohrnii. For the already guaranteed grant of VeChain he also takes over a large part of the development. He is also studying Computer Science at the University of Bern. 

Paula and João are blockchain developers and have contributed heavily to the implementation of Dohrnii. They are and have also both been involved in SayNode Operation's other projects. Paula has a Bachelor's degree in IT Security and a Master's degree in Cryptography, Data Security and Blockchain and previous work experience. João has a Master's degree in Electrical and Computer Engineering and has worked as a Software Developer at Siemens Logistics. From May, Paula and João were joined by Riccardo Mazzucchelli who also has a background as a developer and had his own company in the crypto field. 

Francesco Romeo is a FullStack Developer and has a university degree in Computer Engineering. He has several years of experience as a developer in different companies and accompanied as CTO and Founder the startup Buytime. The last years he worked as a FullStack Developer at the University of Applied Sciences in Bern. 

Simon Heer has worked several years in B2B Sales for RedHat and VmWare as well as in IT Risk and Compliance at AXA Insurance. He has a Master in Digital Business and Innovation and is responsible for the business aspects of the products. 

Ruthusanth Vijayakumar brings loads of experience in application testing and testing management, as well as in business-related areas such as marketing, planning and managing projects. He is currently studying a Bachelor of Science in Business Information at the Bern University of Applied Science.

### Team Code Repos

- https://github.com/SayNode  A few repositories are private because of confidentiality agreements
- https://github.com/RsTs23
- https://github.com/wernerliechti
- https://github.com/YannMarti
- https://github.com/paulamstutz
- https://github.com/RuthuV96

### Team LinkedIn Profiles

- https://www.linkedin.com/in/renato-sch%C3%A4r-8a9a19a5/
- https://www.linkedin.com/in/werner-liechti-568b19213/
- https://www.linkedin.com/in/paula-amstutz/
- https://www.linkedin.com/in/joaogmorais/
- https://www.linkedin.com/in/francesco-romeo-2867083b/
- https://www.linkedin.com/in/riccardo-mazzucchelli/
- https://www.linkedin.com/in/simon-heer-202866110/
- https://www.linkedin.com/in/ruthusanth-vijayakumar-19a7b5189/

## Development Roadmap 

### Example Roadmap for a dApp Application

#### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3 | Milestone 4 | Total |
| - | - | - | - | - | - |
| Estimated Duration | 20 d | 45 d | 30 d | 20 d | 115 d |
| Full-time equivalent (FTE) | 1 | 2 | 1.5 | 1.5 | 6 |
| Cost (up to $ 30,000) | $ 2,500 | $ 14,900 | $ 7,500 | $ 5,000 | $ 29,900|


#### Milestone 1 — User Interface

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Planning | We plan the different Screens of the App |
| 2 | Figma App | We create a UI in Figma of the App to keep an overview and simplify the work with different people. |
| 3 | Figma Website | We create a UI in Figma of the Website to keep an overview and simplify the work with different people. |


#### Milestone 2 - Smart Contracts

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Planning | We plan the architecture of the different Smart Contracts |
| 2 | Developing | We develop the Smart Contracts |
| 3 | Testing | We test the Smart Contracts on the VeChain Test Net |
| 4 | Deployment | We deploy the Smart on the VeChain Main Net |


#### Milestone 3  —  App / Web logic

| Number | Deliverable | Specification |
|-|-|-|
| 1 | App on Goolge Play Store / App Store | We develop the App logic with Flutter and deploy it in the different Stores |
| 2 | Website | We host the Website and implement the possiblity to connect your VeChain Wallet |


#### Milestone 4  —  Marketing

| Number | Deliverable | Specification |
|-|-|-|
| 1 | Planning | We will do a schedule on how often we want to inform our community. |
| 2 | Preparation | In order to keep the community busy through our channel, we will prepare additional advertising material to feed our channels with news and information. |
| 3 | Setup | We set up new accounts for our external channels. The sole purpose for those accounts are to keep connected with the community and to provide the user with information. |



### Community engagement

For community engagement, we will operate different channels simultaneously to achieve the widest possible reach.
 
Website & App: We will use and manage a website and a smartphone application for the platform itself. The website and the app are our core product to sell to our users and customers.
 
External Channels: To reach our customers and to get more people involved into our guessing game, we will intensely use our distribution channels. We will reach for the local newspaper to do a PR-campaign to motivate locals to get involved.
Most of our marketing resources will be used for posting social media content on platforms such as Twitter, Instagram, Facebook and TikTok and Reddit. The social media channels will be prime platforms for our customers to interact with. We will use these channels to do advertising and posting results and rankings of our guessing game. We use these channels for presenting our sponsorship with VeChain as well.
With Reddit and Discord, we want to reach out and manage our growing community. On our LinkedIn page, we will post information about our development and about the product itself for additional promotion for our company SayNode Operations AG.
 
Paid Ads: In order for us to achieve a large reach, we must also resort to paid advertising. For this we will use Google Ads and Facebook Ads. In order to achieve a certain impact, we assume a campaign over several weeks.


## Future Plans

The project should be the cornerstone and at the same time the proof-of-concept for further projects. This way, we can offer the platform for future events to place bets via VeChain. We are thinking especially of UFC, as VeChain has already made a big contribution there. We will also look into other events such as the European Championship or Esports tournaments. The platform can be expanded to include NFTs, for example. 

## Additional Information 

- What work has been done so far?

At this stage, we have developed the business case. We have also clarified the first legal requirements. 
For the UI we have already created first mockups (visual).

- Are there any teams who have already contributed (financially) to the project?

No.

- Have you applied for other grants so far?

Yes, we have requested VeChain grants in the past, but not for this project. 
# VeChain General Grant Application Template

## Project Overview 

- Project: SW3 (“WEAR & W3N”)
- Team Name: Kek Labs
- Payment Address: 0x3D4bdEB3C43D3792e6fF7A29309D07CE7053Ec26 

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

Please provide the following:
- **A brief description of the project:**\
SW3 powers the digital heirloom ecosystem. We help people create digital memories and tie them to their favorite mementos, pieces of clothing, jewelry, and more. SW3 is a platform where users can connect their items to manage their on-chain memories, sell their heirlooms, and customize their collections for others to view. The platform is powered by our protocol that ties physical objects to their on-chain counterparts.
- **An indication of why your team is interested in creating this project within the VeChain Ecosystem:**\
We’re excited at the prospect of working within the VeChain ecosystem because of the longevity of VeChain’s economic model (meaning you’ll be here for the long haul), the values that VeChain’s ecosystem presents, such as the drive to create interwoven systems into previously isolated or inaccessible ecosystems, the desire to maintain a technology that **positively** impacts the world we live in, and the network of projects and teams working to make VeChain a great ecosystem to work in (from VeFam to VPunks and everything in between!). We have had great experiences with VeChain, including hosting your social arm recently on our Twitter Spaces hosted with WhaleCoinTalk/TheAquarium/MobyMedia, and working together in the Phygital web3 realm in the past.
- **If relevant, an indication of how you will integrate tools and features (e.g., Sync2/Connex, fee delegation protocols, MTT, etc) to enhance your project**:\
 We’ll use Connext to support multiple wallets (Sync, Sync2, VeChainThor Wallet) and MPP to support on-chain data in the form of the memories tied to an heirloom. MTTs are going to be implemented to account for a user adding multiple memories at once to single or multiple heirlooms. We were also exploring using transaction dependency and want to know the extent to which it can depend on. We need the objects to exist and memories not to be created but it looks like it’s transactional. Definitely have questions there! We’ll also keep an eye out for marketplace tooling that we can integrate with rather than build our own, if possible.

### Project Details

We expect the teams to already have a solid idea about the project's expected final state.
Therefore, we ask the teams to submit (where relevant):
- Mockups/designs of any UI components:\ We’re mocking up the front end and can submit some core screens over the next 2 weeks.
- API specifications of the core functionality:\
getHeirloomById - gets a specific heirloom\
getHeirlooms - gets a list of all heirlooms\
getHeirloomByUser - gets a list of all heirlooms from a user\
postHeirloom - creates an heirloom\
putHeirloom - updates an heirloom\
postMemoryById - posts memories to a specific heirloom\
getHeirloomMemoriesById - gets memories attached to a specific heirloom\
getUserGallery - gets a specific user’s gallery\
getUserProfile - gets a specific user’s profile\
postUserProfile - creates a user’s profile\
putUserProfile - updates a user’s profile\
postUserGallery - creates a user’s gallery\
putUserGallery - updates a user’s gallery\
**Might not be needed, but all the end points associated with the marketplace:**\
postHeirloomSale - Create a posting on the marketplace for an heirloom\
putHeirloomSale - updates a posting on the marketplace for an heirloom\
deleteHeirloomSale - deletes a posting on the marketplace for an heirloom
- An overview of the technology stack to be used:\
The app is to be built in React with a Next backend. We’ll use Postgres for any database need and AWS for our hosting provider. Serverless functions will be positioned in Lambda as needed.
- Documentation of core components, protocols, architecture, etc. to be deployed
- PoC/MVP or other relevant prior work or research on the topic

### Future Plans

**Please include the team's long-term project plans, operation plans and intentions:**\
The team will be implementing the technology across multiple products, expanding from our initial offering of just wearables. The product is being built to accomplish the goals of enhancing physical goods with digital capabilities by utilizing blockchain technology to solve the larger goals of creating downstream revenue-share and data access for brands and manufacturers. SW3 specifically recognizes the most important issue of the NFT being the method of transfer. 

Most phygital projects utilize blockchain technology simply to authenticate products and to confirm provenance. SW3 does this as well, fundamentally, but in order to get the invaluable benefits of downstream consumer data and royalties from downstream sales, the NFT must be the method of transaction, and SW3’s value-proposition of the NFT with added memories, embedded into the physical good, makes the method of transfer the NFT and not simply the physical object. 

Short term plan is to integrate NFC chips into physical products of existing partners and customize Wear & W3n app for partners. We will formulate activation and gamification strategies for each partner that will maximize their brand loyalty and product experience which will consumers will engage with via the custom-app that they are directed to via the NFT embedded into the NFC chip. 

We will also be integrating our product into other phygital products that all only focus on provenance and authentication (static experience experience that exists primarily at the time of purchase/redemption) while we provide the phygital experience for the life of the product post-purchase, which is the true massive data, financial, and loyalty opportunity for brands.


#### Long-term project Plans

**Please include information about any future development plans that the team has:**\
The team wants to open up the protocol after proving the model works, creating a new heirloom/memory economy. Imagine being able to purchase an heirloom from Kendall Jenner, tied to her personal memories that she made while wearing it and you had the power to share those memories or keep them to yourself. Or imagine a mother passing her wedding ring on to her daughter, and her daughter to hers, each not having to tell the story of their marriage and love, but with the memories embedded into the ring. Turning items into heirlooms by permanently etching moments into memories via the immutability of the blockchain. 

We also want to make it easy for people to have the tools to choose what they want to create as an heirloom. We are initially partnering with some larger creators and communities, but want to build the tech and logistical infrastructure to be able to offer a kit/system for users to implement on their own, or deploy within their own companies/projects.


#### Business / Operation Plans

**If you are applying with a dApp, infrastructure, or service, please provide details about your business / operational plans:**\
The product has been described throughout this application. Also, see SW3 DECK for more details. The business/operational plans are, briefly, as follows. 

The value-add potentials of phygitals are undeniable. The question is how do you implement seamlessly and cost-mindful into brands and products with an effective solution that causes industry disruption without causing operational or brand disruption with the individual brands or companies?

The answer is simple if one truly understands the technology, business in general, and the hurdles/expectations/appetite of the businesses you intend to implement into.

As described herein, the value proposition is that brands barely even know where their products are at any given time in the supply chain, and even less often who the end store or buyer is. They certainly do not usually have any idea who is buying/selling on secondary markets, nor earn any revenue from it, nor even the data of the people/purchases/pricing beyond initial sales.  We have spent years talking and working with brands and manufacturers to confirm the massive desire to capture pieces of the revenue/data/loyalty potentials on secondary markets or sales, but they are either afraid of the efforts and cost associated with creating and implementing their own solutions (marketplaces, etc), and have already built their business models around the absence of this capture. 

When one speaks with brands about integrating web3 strategies into their brand, the push back is usually a blend between a fear of stigma to the brand, fear of costs, fear of lift, and simple disinterest due to the perceived friction/effort associated with any such perceived massive friction to fundamentally change the business model.

That is where our years of combined web2, web3, and phygital experience comes in. Our product requires no change to the brands business model. NFC chips (no cost to brand) is implemented into the products in the manufacturing process (partnering with manufacture friends). No impact on product cost. The NFTs are already backed into the NFC chips if/when the brand wants to activate a web3 consumer/product/brand strategy. We work with the brand to skin our native white-glove app to feel native to the brand. We work with the brand to devise the most impactful, desired, effective Phygital strategy. When ready, the brand launches the campaign that informs its consumers (“holders”) of the added phygital capabilities of the products they already own. Think Nike: “to holders of X t-shirts, you can now tap your phone on the Nike logo (NFC chip embedded under logo) to access a new virtual world of rewards, giveaways, and opportunities connected to adding your life into your t-shirt (NFC chip has link to download app, and once downloaded, customer claims ownership of t-shirt NFT as they setup their SW3/Nike “Wear & W3n” app). More explanation to come, but for the time being, please tap your t-shirt, download the app and follow the instructions (actions now exists via the customer to the item, and the item to the app, and Nike can communicate, activate, and incentivize their holders however they would like, in perpetuity).” - the action of tapping and adding memories is rewarded with points/tokens/rewards.

The goal is MINIMIZING FRICTION:
-minimal lift for brands and consumers
-creating new avenues of connection and loyalty
-incentivizing the creation of content to personalize products
-incentivize the transfer of products to be via the NFT by making it the value-add component of the item

Once brand and consumer are used to the action set, the potentials are endless (with the help of tokenization and gamification) in terms of capturing new data, money, loyalty, and gamifying the real world from a brand-centric lens - the likes of which will shift both digital and physical consumption forever.



### Ecosystem Fit
Are there any other projects similar to yours? If so, how is your project different?\
There are a number of phygital projects that exist. We have been in the phygital space for many years and have been working aggressively, via socials and other marketing avenues, to create awareness of the potential for a phygital future. When we started most people either laughed at the word “phygital”, dismissed the potential, or could not understand the concept. Slowly but surely phygital projects started entering the market, but they were mostly gimmicks and benefited from the attention that anything “different” gets in the Bull market. 

However, we were not interested in cash grabs or gimmicks. 

About 2 years ago we launched an introductory NFT art project in honor of Kobe Bryant in partnership with NiftyGateway (OpenEdition mint @ $240. Sold 225 units. Elite group of NFT and art collectors purchased the majority of them and the floor price sat at around 15X mint price for over a year. Floor price currently sits stable at 5X+).

Over the past 2 years, while we were working hard to create the market for phygitals, and thereby product-market-fit for SW3, we watched phygital projects launched that were increasingly less and less gimmicky, but none have gone beyond the initial consumer purchase by offering the utility of authentication and provenance.

SW3 also authenticates and proves provenance, but its true goal is to bring utility, value, and new economic models for brands and manufacturers by adding blockchain technology benefits to the LIFE of the physical, far beyond the moment of purchase. This is the Holy Grail: brands having never-before captured data, money, and connectivity not just to the initial buyer, but for the life of the buyer, and all future downstream buyers of the same single product.

We’re different because we aren’t:
Fractionalizing ownership
Making a strong play to get user data to better their experience. We already have the value prop set forth and want to eat our own dog food to prove the model before opening it to the public.
Have a strong core team
Selling NFT’s
Using “phygital” as a tag phrase or gimmick
Requiring web3 experience/knowledge
Foolishly trying to pretend we are manufacturers and making the products ourselves
Figuring it out as we go (extensive experience in web3 and phygital technology)
Charging the customer
Altering the manufacturing process dramatically
Introducing any friction to existing business models of brands
“Hype-driven”
Children (we are seasoned successful businessmen from web2 and web3)

## Team 

### Team Members

- Name of team leader\
Phygital (Shawn Goodman)
- Names of team members\
Aaron Guyett\
Sam Turner\
Jayde Herrick

### Team Website

- www.sw3nft.com
- www.sw3nft.io

### Team's Experience

Please describe the team's relevant experience. If the project involves development work, then we'd appreciated it if you can single out a few interesting codes commits made by team members on their past projects.

Aaron has launched or been a part of numerous projects both in and out of Web3. Originally in school for neuroscience, Aaron taught himself development, built applications for medium and large businesses while working at AWS, taught software engineering and AWS at University, led the Risk and Compliance team at a 5,000 person financial services firm, launched two funded startups as CEO/CTO (1 exited), secured a large grant to build infrastructure for Klaytn Foundation, created the Quarter Machine IRL experience (https://quartermachine.io), and has a long list of projects in Web3 he’s been a fully-doxxed-part-of; some of them are: Unnamed.gg, mintpass.com, thenftarcade.io, myseedstarter.com.

Shawn has been involved in Blockchain for nearly a decade. He was a late co-founder of a real world phygital company for several years and has been the leading public voice of the phygital future for the past 5 years. He featured his phygital solutions and creations at Art Basel a few years ago, phygitizing an entire gallery, and displaying his Kobe NFT in a Hologram PORTL unit at Art Basel and around the United States. He has a wealth of real world business experience (bars, restaurants, real estate) and has founded numerous startups and iOt products. Shawn has consulted and partnered with a number of successful web3 projects and has contributed to the future of core web3 infrastructure with the likes of Yuga, A Kid Called Beast, HalfBAYCD, Froopyland, SaaSy Labs, Mutant Grape Wine Club, and many more. He also regularly hosts the largest web3 twitter spaces, has deep relationships throughout the web3 ecosystem, and has deep ties with real world companies in various industries/niches, including eBay, Walgreens and many more.


### Team Code Repos

Not yet relevant for the project.

### Team LinkedIn Profiles

- https://www.linkedin.com/in/aarondguyett

## Development Roadmap 

This section should break out the development roadmap into a number of milestones. Since the milestones will appear in the grant contract, it helps to describe the functionality we should expect, plus how we can check that such functionality exists in the product. Whenever milestones are delivered, we refer to the contract to ensure that everything has been delivered as expected.

Below we provide an <b>example roadmap</b>. For each milestone:

- Please indicate the milestone duration, workload in terms of full-time equivalent (FTE) and cost. 
- Please be sure to include a specification of the software. The level of details must be high enough so that we are able to verify that the software meets the specification.
- Please note that we require documentation (e.g. tutorials, API specifications, architecture details) in each milestone. This ensures that the code can be widely used by the community.
- Please provide a test suite, comprising unit and integration tests, along with a guide on how to run these.
- Please commit to providing dockerfiles for the delivery of your project.


### Roadmap for SW3

#### Overview

|   |  Figma Prototype | Initial Frontend MVP | Smart Contract Build | Total |
| - | - | - | - | - |
| Estimated Duration | 14 d | 25 d | 16 d | 55 d |
| Full-time equivalent (FTE) | 1 | 4 | 2 | 7 |
| Cost (up to $ 30,000) | $ 6,500 | $ 12,500 | $ 11,000 | $ 30,000 |

> *⚠️ Please note that milestone 1 funds cannot exceed 40% of the total amount you are applying for.*

#### Milestone 1 — Figma Prototype

| Number | Deliverable | Specification |
|-|-|-|
| 0a. | Documentation | The labeled Figma prototype will be very detailed and highly engaging while showcasing a fully-functional app. |
| 0b. | Brand Kit | The brand kit included with this will be the base for the theme we create as well as the logo and wordmakr we use. |
| 1 | Wireframes and Moodboard | The Figma prototype stems from the wireframes created for the project and the associated moodboard as a guideline. |
| 2 | Prototype | The clickable prototype includes all functionality needed to create the application for the dev team. The development team can start coding in tandem with the design team. |

#### Milestone 2  —  Frontend MVP
| Number | Deliverable | Specification |
|-|-|-|
| 1 | Frontend Application | The frontend application is to be built with basic functionality from the prototype. Final features are to be included after the initial build. Things like the marketplace are excluded. |

#### Milestone 3  —  Smart Contract
| Number | Deliverable | Specification |
|-|-|-|
| 0a. | Documentation | Documentation for each smart contract is created in line with our testing suite before we begin developing code. It is adjusted throughout development. |
| 0b. | Testing | We develop with testing in mind, so we create our test cases first and build for them. |
| 1 | Smart Contract | The first of a few smart contracts is to be built and tested. The smart contract tied to our physical product is built at this stage to ensure users can create heirlooms and memories. |


#### Community Engagement

As part of the Program, we require that you produce and publish at least one article/tutorial (e.g., on Medium). It should explain your work done as part of the grant. 

We recommended you provide social medium, like Twitter, Telegram group, or Reddit, on your website. When the developers/users need assistance, they could get in touch with you and get help.

We have posted and talked about phygitals ad nauseam on social media, at web3 events, and to investors/chains/industry titans. We can provide evidence of the above, and certainly document the article and related requirements detailed in the question above.


## Additional Information 

Any additional information that you think is relevant to this application that hasn't already been included.

Possible additional information to include:
- What work has been done so far?\
There’s a protocol that we created that exists but needs some restructuring to fit the project a bit better. The protocol saves the dev team a ton of time.
- Are there any teams who have already contributed (financially) to the project?\
No external funding. All funding has come from existing internal team members (self-funded)
- Have you applied for other grants so far?\
No, our sights are set on VeChain. I’ve worked on many, many other chains and although they all have their pros and cons, I want to work on a chain that supports sustainability and isn’t just thinking about the degen boom. I also appreciate many of the protocols and attention to detail the dev team has towards other devs. It feels like every update helps us more and more. Most importantly, VeChain is the pioneer in phygital solutions and the use of blockchain technology to solve supply chain problems. In fact, besides for working with VeChain in the past, we hosted VeChain on socials and specifically sought out ONLY VeChain for grant or financial support.

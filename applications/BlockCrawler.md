# VeChain General Grant Application Template

## Block Crawler

- **Project Name:** Block Crawler
- **Team Name:** ZettaFi Labs, Inc.
- **Payment Address:** 0xC0Efea6aa8947fC2F207333FE2F61a79069392ac

## Project Overview :page_facing_up:

### Overview

- Block Crawler is an open source high-performance ETL framework for blockchain data designed to process blockchain data and transform it into useful datasets in the easiest way possible. We will configure it for free to collect any dataset for you.
- Block Crawler creates datasets from blockchains and provides it to those who are building applications. Its high-performance, open-source ETL framework is designed to process massive amounts of blockchain data and transform it into useful datasets in the easiest and most expedient way possible. With Block Crawler, anyone can extract any blockchain data from EVM RPC APIs like Ethereum, Polygon, and more, transform it into desired datasets, and persist it into databases to support data access requests on historical and real-time data. Furthermore, the Block Crawler's modular components can be combined with dataset specific components to cater to the unique requirements of every user.
Whether a blockchain looking to improve data availability or a blockchain application needing a specific dataset, we are creating a product where data consumers tell us what data they need, and we configure the Block Crawler for them and work with them to extract, transform, and load the data.
- It will allow you to extract any dataset from any blockchain you might find valuable now and into the future. This will ensure you have access to the data you need to display the complex analytics dashboards, make important internal business decisions and analyze on chain behavior. We can load any historical dataset you want into a database to perform data science as well as loading real-time data into a database you can query with an API.
- Our mission at ZettaFi Labs is to empower the world to trustlessly connect and deliver all available data in every useful form in the most convenient and reliable way. 
### Project Details

We expect the teams to already have a solid idea about your project's expected final state. Therefore, we ask the teams to submit (where relevant):

- We are hoping to accomplish the goal of improving accessibility to valuable datasets. We would define success for this grant to be extracting, transforming and loading valuable datasets from any blockchain into a database of your choice. The scope of the grant would depend on the volume and complexity of the datasets requested. We would consider this project successful if we improve data accessibility in the blockchain industry. While open-source data extraction tools for overly generic or specific niches are emerging, there is currently no high-performance framework for creating and maintaining robust datasets from Blockchain data.
- The core of the Block Crawler is a high-performance parallel processing data bus that allows data to be passed between the various components implemented. First, data is fed to the data bus which provides the data to the various components that transform the data and feeds it back into the data bus. This transformation process continues until the data has reached its final form and is then persisted.
***Example: Let's propose we want to load all NFT transfers for all contracts in an Ethereum blockchain. Because we don’t know the address of every contract in a blockchain, we would need to process every block that may have transfer information. The data bus would be fed what we do know, which is block numbers. Then, the data bus would pass the block number to components that would transform block numbers into blocks, transform blocks into transaction receipts, transform the log entries from transaction receipts into NFT transfer records, and finally persist the NFT transfer records to a datastore. This process is optimized by processing the transformations and persistence in parallel.***
- We used the Block Crawler to extract, transform and load all NFT data from the Ethereum mainnet in two weeks. Then, we made that data available via API for anyone trying to build utility for their NFT project or game. We are now looking to increase usage of our product by identifying additional datasets the blockchain industry would find valuable to index and implement the Block Crawler to extract them. 

### Ecosystem Fit

- We are hoping to accomplish the goal of improving accessibility to valuable datasets. We would define success for this grant to be extracting, transforming and loading valuable datasets from any blockchain into a database of your choice.
- Block Crawler is versatile, allowing you to extract any dataset from any blockchain you might find valuable now and into the future. This will ensure you have access to the data you need to display the complex analytics dashboards, make important internal business decisions and analyze on chain behavior. We can load any historical dataset you want into a database to perform data science as well as loading real-time data into a database you can query with an API.
- The initial configuration and consultation would be free and the software is open source. We have a team of 6 engineers working to increase data availability in the blockchain industry. The funds would be used to shift the focus of those team members from their usual day-to-day activities to fulfilling the requirements of our engagement. This cost is variable depending on the scope and level of skill necessary for your needs.  

## Team :busts_in_silhouette:

### Team members

- **Yo Sub Kwon** is the CEO of ZettaFi team and has co-founded Coinsetter, which was acquired by Kraken and LaunchKey and is now owned by TransUnion. He started mining Bitcoins in 2010 and also co-founded Hosho Group, a smart contract security analysis firm in 2017. 
- **Cylus Watson**, CSO, is a serial entrepreneur in the blockchain space, having launched a consulting firm and two hedge funds with consistent success in identifying and capitalizing on trends, as well as being a leading yield-farming expert. 
- **Adam Englander**, Director of Engineering, is the founder of two successful developer groups and maintainer of Pallets (including Flask). He is also a voting member of the Python Software Foundation and a global speaker on cybersecurity.


### Contact

- **Contact Name:** Yo Sub Kwon
- **Contact Email:** grants@zetta.fi
- **Website:** https://zetta.fi/

### Legal Structure

- **Registered Address:** 919 North Market Street, Suite 950 Wilmington, Delaware USA 19801
- **Registered Legal Entity:** ZettaFi Labs, Inc.

### Team's experience

In addition to the experience listed under **Team Members**, our team consists of nine full-time staff members who work remotely globally. This includes six engineers with multiple proficiencies in cybersecurity, blockchain technology, distributed systems, and large-scale systems. The engineering team has reputable distinctions as maintainers of highly popular open-source projects, founders of developer groups, and regular speakers at events worldwide.

### Team Code Repos

- https://github.com/block-crawler

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- https://github.com/jchysk
- https://github.com/aenglander

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/jchysk/
- https://www.linkedin.com/cylus-watson-064190157/
- https://www.linkedin.com/adamenglander/

## Development Status :open_book:

- https://drive.google.com/file/d/1Wcfz3Yr9ybrWAvblFhpyq__L8uYxeK7K/view?usp=share_link
- https://block-crawler.readthedocs.io/en/latest/api-reference/index.html

## Development Roadmap :nut_and_bolt:

We are currently doing market research into what datasets are difficult to extract from blockchains and are considered valuable. Our open source software is capable of being configured to extract, transform and load any dataset but we are still unsure about which datasets the industry considers most important to extract. Depending on the volume and complexity of that data extraction, the cost and future milestones would be impacted/determined. The initial consultation and configuration of Block Crawler is free. We will work with your team to identify important datasets, configure the Block Crawler for you to extract those datasets and assist you with loading those datasets into the database of your choice. After this initial milestone, the long-term engagement would depend highly on the project's scope and specific needs. 

The initial configuration and consultation would be free and the software is open source. We have a team of 6 engineers working to increase data availability in the blockchain industry. The funds would be used to shift the focus of those team members from their usual day-to-day activities to fulfilling the requirements of our engagement. This cost is variable depending on the scope and level of skill necessary for your needs.  

### Overview

- **Total Estimated Duration:** Average 2 months, depending on dataset requested
- **Full-Time Equivalent (FTE):**  We have a team of 6 engineers able to work on this depending on its scope.
- **Total Costs:** We are offering the initial configuration and consultation for free and the software is open source. After the free initial engagement, we would be looking for anywhere from $10k USD to $50k USD depending on the scope of the ongoing work. 

...
## Future Plans
Our team is committed to the long-term success and sustainability of Block Crawler, and we have devised a comprehensive plan to maintain and upgrade the software over time, ensuring its continued value to the blockchain ecosystem:
- Regular Maintenance: We will allocate dedicated resources to perform routine maintenance, including bug fixes, security patches, and performance optimizations. This will ensure the software remains secure, stable, and efficient for its users.
- Continuous Development: Our development team will actively work on implementing new features, enhancing existing functionalities, and incorporating feedback from the community. This will help us keep the software relevant and up-to-date with the evolving needs of the blockchain ecosystem.
- Ecosystem Integration: As new blockchains and technologies emerge, we will prioritize integrating Block Crawler with these platforms, ensuring broad compatibility and maximizing its utility for users across various networks.
- Open-Source Collaboration: By maintaining an open-source approach, we will encourage contributions from the wider community, fostering collaboration and shared learning. This will enable us to continuously improve Block Crawler with diverse perspectives and expertise.
- Documentation and Support: We will keep documentation updated and comprehensive, allowing new and existing users to understand and utilize Block Crawler effectively. Additionally, we will provide ongoing support through various channels, such as community forums, email, and social media, to address user concerns and queries.
- Funding and Partnerships: To support the long-term growth of Block Crawler, we will actively seek funding through grants, sponsorships, and partnerships with key stakeholders in the blockchain industry. This will help ensure we have the necessary resources to maintain and enhance the software over time.
- Monitoring and Evaluation: Our team will regularly assess the impact of Block Crawler on the blockchain ecosystem and use these insights to guide future development priorities, ensuring the software continues to address the most pressing needs of its users.

By implementing these long-term plans, we aim to maintain and upgrade Block Crawler over time, ultimately contributing to the growth, innovation, and sustainability of the broader blockchain ecosystem.


## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?**  Website

- We are currently doing market research into what datasets are difficult to extract from blockchains and are considered valuable. Our open source software is capable of being configured to extract, transform and load any dataset but we are still unsure about which datasets the industry considers most important to extract. In addition to financial support, or even instead of financial support, we would appreciate the ability to ask some questions about your data needs and any pain points you have experienced when dealing with blockchain data. 
- Please read our one-pager: https://drive.google.com/file/d/1Wcfz3Yr9ybrWAvblFhpyq__L8uYxeK7K/view?usp=share_link

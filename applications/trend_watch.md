# VeChain General Grant Application Template

## Project Overview 

- Project: Trend Watch
- Team Name: greenfield-br
- Payment Address: 0x78F932824880505690B9e14Cb0097aA3E3B7Fe00

> ⚠️ *The combination of your GitHub account submitting the application and the payment address above will be your unique identifier during the program. Please keep them safe.*

### Overview

Please provide the following:
- A brief description of the project.

Vechain has been chosen by relevant projects as their blockchain. Their tokens are an import financing venue. However, many of these projects are not well known by the broad public. This inhibits trading volume, dries out liquidity and potentially hurts their financing cycle.

Oceanex is a centralized exchange with a unique offer of VET quoted pairs. Vexchange on the other hand, is a decentralized exchange (DEX) accessible directly from the Vechain Thor Wallet, the official wallet of Vechain Thor. Oceanex provides rich trading information while Vexchange is readily accessible from the Vechain Thor Wallet.

In the crypto trading community, amongst many doubts, many do not have a clear idea of what and when to trade.

At Greenfield, since 2013 we've been developing price forecasting tools (see http://www.ucs.br/etc/revistas/index.php/scientiacumindustria/article/view/5746/pdf for our, then, early results; https://youtu.be/MDtgRp5ZH10 for a live demo, and https://youtu.be/bTUDd_iVJ5A for a detailed explanation) that evolved to trading strategies (see https://youtu.be/QVPSU3GEFd0 and https://youtu.be/2edd7YGPJdQ) relying on open source projects as CCXT.

We want to build a multi chart monitoring panel of VIP180 tokens / VET pairs. Trading data from Oceanex will be queried and processed by widely accepted trend following indicators (for instance, moving average crossings and ichimoku clouds) with resulting buy/sell indications. Upon connecting his/her wallet, the user will have the option to directly swap available VET balance by the corresponding VIP180 token and vice versa.

With this project we intend to showcase to crypto trading community Vechain based projects, as well as providing them with a ready to trade environment. We believe it'll both engage existing users as well as attracting new ones, boosting the network effect in the long run.

- An indication of why your team is interested in creating this project within the VeChain Ecosystem.

Different from more well know projects, Vechain has a lot of room to grow and we believe our project can make a difference in its expansion.

We believe decentralized trading is the near future and we know not of any other blockchain ecosystem that combines
- solid long term growth perspective,
- real case application projects (as JUR and SHA, for instance),
- current liquidity deficit,
- low cost transactions and
- straightforwardness in development.
We can cite other ecosystems, as Waves, EOS and Ethereum, for instance. But we believe each of them underperforms Vechain in at least one of these items.

- If relevant, an indication of how you will integrate tools and features (e.g., Sync2/Connex, fee delegation protocols, MTT, etc) to enhance your project. 

Our application will work as follows
- download trading data from Oceanex through K-lines API calls,
- if appropriate, market data availability will be checked through CCXT API calls prior to K Lines get request.
- plot respective VIP180/VET charts in a 3x2 grid (2 lines, 3 columns)
- process these data through a series of commonly accepted buy and sell rules for trend following (moving average crossings and ichimoku clouds; possibly 1H, 1D, 1W charts)
- synthesize indicator outputs in an intuitive scoreboard bellow the charts ranging through sell, neutral and buy.
- through connex, visitor connects his/her wallet and charts are customized to the assets on his/her balance
- buy and sell widgets displayed bellow each chart allow for swaps on vexchange (connex).


### Project Details

- Mockups/designs of any UI components

Main Trend Watch Panel page
https://greenfield-br.com/wp-content/uploads/2021/09/htmlPage.jpg

Detailed info page for each chart
https://greenfield-br.com/wp-content/uploads/2021/09/detailedInfoPage.jpg

- API specifications of the core functionality

Oceanex K Line API specification taken from https://api.oceanex.pro/doc/v1/#k-line-post

import requests
method_url = base_url + "/k"
data = {
  'market': 'btcusdt',
  'limit': 2,
  'period': 5,
  'timestamp': 1559232000,
}
r = requests.post(method_url, data=data)
The above command returns JSON structured like this:

{
  "code": 0,
  "message": "Operation successful",
  "data": [
    [1559232000,8889.22,9028.52,8889.22,9028.52,0.3121],
    [1559232300,9052.86,9052.86,8971.44,8996.5,0.1469]
  ]
}

Connex.Thor Account Visitor API specification taken from https://docs.vechain.org/connex/api.html#account-visitor

const acc = connex.thor.account('0x7567d83b7b8d80addcb281a71d54fc7b3364ffed')

- An overview of the technology stack to be used

Server, linux ubuntu 20.04 / nginx
Application Development, Python3.8 / python-devkit.py

- Documentation of core components, protocols, architecture, etc. to be deployed

Python standard modules as data processing tools
https://pandas.pydata.org/
https://numpy.org/
https://www.scipy.org/

Python CCXT wrapper as market verification data (possible deployment)
https://github.com/ccxt/ccxt
https://github.com/ccxt/ccxt/tree/master/python#install

Python wrapper for TA-Lib as technical analysis library
https://mrjbq7.github.io/ta-lib/

Plotly as Chart library
https://plotly.com/python/

Thor Devkit as VeChainThor blockchain interaction
https://github.com/vechain/thor-devkit.py

- PoC/MVP or other relevant prior work or research on the topic

Time Series Forecasting Tool. Python/CCXT cli app.
https://github.com/greenfield-br/wildhorsesForecast
This project illustrates our ability in gathering data with API calls on exchanges, processing (OHLCV) data from a trading perspective and building visualizations that synthesize the core of the info (see https://youtu.be/Lb7jR-Kzyjk for a live demo).
It was released in Jul/17 and deployed until Nov/19.

Long Short (Pair Trading) Arbitrage Bot
https://github.com/greenfield-br/longShotArbitrageBot
This project illustrates our ability to connect to an exchange through API calls, authenticate and trade.
The code was writen to ensure timely execution of orders (see https://youtu.be/2edd7YGPJdQ for a live demo).
Despite being an arbitrage bot, it succeded with API calls instead of standard websockets.
It was deployed from Feb/19 until Aug/19 when arbitrage stopped being profitable.

### Ecosystem Fit
Are there any other projects similar to yours? If so, how is your project different?

There are several similar projects. To cite a few, Metatrader 5, TradingView, Tabtrader, Vexchange.
- Metatrader and TradingView do not connect to Oceanex for data reading.
- Tabtrader does not connect to Vexchange for swapping.
- Vexchange does not provide price action information.

Whereas we
- connect to Oceanex for data reading,
- provide price action information and
- connect to Vexchange for swapping.

Despite that, we raise awereness of VIP180 tokens and stimulate usage of VeChainThor Wallet.
A link for VeChainThor Wallet download is included in the panel design.

## Team 

### Team members

- fernando augusto bender, project leader.

- Guilherme Keiel, head of development.

- Gustavo Pozza, head of UX/UI.

### Team Website

- https://greenfield-br.com

### Team's experience

Me (fernando bender) and Guilherme Keiel have been working together since around 2015, where I've supervised his academic research in cloud computing time series research (see https://www.researchgate.net/publication/301234963_Identificacao_de_sistemas_aplicado_a_maquinas_virtuais_uma_experiencia_com_KVM_Xen_e_modelos_ARIX).

The results were then applied to financial time series (see https://www.researchgate.net/publication/323055166_Modelagem_de_series_temporais_financeiras_uma_abordagem_estatistica_para_a_identificacao_de_modelos_de_media_condicional).

The next step was developing a tool for price forecasting (see https://github.com/greenfield-br/wildhorsesForecast), which upon success naturally led our company to a trading bot (see https://github.com/greenfield-br/longShotArbitrageBot).

Its successful deployment sparked its SaaS distibution in 2019. However, arbitrage profitability in general dried out later on that same year, leading us to long positioning trading bots, instead.

After researching on the most relevant ones we've built visualization tools for backtesting results. This allow us to fine tune strategy parameters through time (see https://github.com/greenfield-br/Optimizer/blob/main/btcusdt_stop_lock.png for an example; contact us for details).

During our product development process we have always designed every step of the solution, developed its core, and hired professionals for complementary tasks, if needed.

### Team Code Repos

https://github.com/greenfield-br/wildhorsesForecast
https://github.com/greenfield-br/Optimizer
https://github.com/gkeiel/gkeiel.github.io

### Team LinkedIn Profiles

https://www.linkedin.com/in/fernandobender/
https://www.linkedin.com/in/guilherme-keiel/
https://www.linkedin.com/in/gustavo-l-pozza-5b338b28/

## Development Roadmap 

#### Overview

|                            | Milestone 1 | Milestone 2 | Milestone 3 | Milestone 4 | Milestone 5 | Total    |
| ---------------------------|-------------|-------------|-------------|-------------|-------------|----------|
| Estimated Duration         | 60 d        | 30 d        | 30 d        | 60 d        | 30 d        | 210 d    |
| Full-time equivalent (FTE) | 2           | 2           | 2           | 2           | 1           | 9        |
| Cost (up to $ 30,000)      | $ 6,000     | $ 4,000     | $ 8,000     | $ 8,000     | $ 4,000     | $ 30,000 |

#### Milestone 1 — Trend Watch Panel + Docker container + Initial documentation

| Number | Deliverable   | Specification |
|--------|---------------|---------------|
| 0a.    | License       | GPLv3         |
| 0b.    | Documentation | We will provide both inline documentation of the code, a tutorial and videos on how to install the application using docker, local install on linux. A link on how to install linux on a virtual machine will be provided.
| 0c.    | Testing Guide | Not applicable. Instead, a troubleshooting guide will be included in the available documentation.
| 1      | Html Page     | A html page will be built for displaying the charts (3x2 grid) from VIP180 / VET pairs as traded in oceanex.
| 2      | Backend       | Periodic API calls to oceanex will be performed in order to update the 1H, 1D, 1W charts.
| 3      | Deliverables  | A docker container will be produced for this initial version, as well as the documentation, and the set of files for local install. Although the functionality of the deliverable is restricted, in this milestone the structure of docker containerization and documentation is produced, being expanded in the next milestones, accordingly.

#### Milestone 2 — Indicators + Detailed info pages

| Number | Deliverable         | Specification |
|--------|---------------------|---------------|
| 0a.    | License             | GPLv3         |
| 0b.    | Documentation       | We will provide both inline documentation of the code, update existing multimedia documentation on how to interpret the trend following indicators included in this milestone and navigate from the main html page to the detailed info pages for specific pairs. 
| 0c.    | Testing Guide       | Not applicable.
| 1      | Updated Html Page   | The html page delivered in the previous stage will be updated to include the scorecards for the trend following indicators.
| 2      | Detailed Info Pages | Each chart will have a link to a detailed page, where the chart is appears expanded, as well as the indicators related info. If appropriate it might contain specific token info, as market cap, total supply, etc.
| 3      | Deliverables        | The previous milestone deliverables will be updated to include current developments.

#### Milestone 3 — Wallet connection

| Number | Deliverable         | Specification |
|--------|---------------------|---------------|
| 0a.    | License             | GPLv3         |
| 0b.    | Documentation       | We will provide both inline documentation of the code, update existing multimedia documentation on how to connect the wallet to the application. Additionally, a link to VeChain website documentation with download, install, usage instructions will be provided.
| 0c.    | Testing Guide       | A testnet wallet will be created, and a tutorial on how to connect it to the application will be provided, in both text and video. 
| 1      | Wallet connection   | A button "Connect Wallet" will be added. It'll connect to wallet, read balances, and customize the charts exhibit, prioritazing the pairs whose balances are not null in the user wallet.
| 2      | Deliverables        | The previous milestone deliverables will be updated to include current developments.

#### Milestone 4 — Swap functionality

| Number | Deliverable         | Specification |
|--------|---------------------|---------------|
| 0a.    | License             | GPLv3         |
| 0b.    | Documentation       | We will provide both inline documentation of the code, update existing multimedia documentation on how to swap your tokens from the application. 
| 0c.    | Testing Guide       | The testnet wallet of previous milestone will be used again for testing the swap functionality, and a tutorial on how to perform it will be provided, in text as well as in video. 
| 1      | Swap functionality  | A call to Vexchange smart contract will be performed estimating the price impact of the proposed swap. Upon approval, a swap request will be issued.
| 2      | Deliverables        | The previous milestone deliverables will be updated to include current developments.

#### Milestone 5 — Application wrap up

| Number | Deliverable     | Specification |
|--------|-----------------|---------------|
| 0a.    | License         | GPLv3         |
| 0b.    | Documentation   | Existing documentation will be revised and concluded. 
| 0c.    | Testing Guide   | Not applicable. 
| 1      | Additional info | Introductory information for new users/visitors will be added, presenting the project, what it is, what it does. This will be done with hyperlinks to additional pages. As a final step before releasing this milestone, an article on Medium about the project and explaining the work as part of the grant will be writen.
| 2      | Deliverables    | The previous milestone deliverables will be concluded.

#### Community engagement

As part of the Program, as mentioned in the last milestone, we will produce and publish one article on Medium. It shall explain our work done as part of the grant.

## Future Plans

We intend to use this project ourselves, publishing it as a website, which we will maintain. We plan to add contact information so visitors can contact us directly. It would be a great showcase for our trading algorithms.

Our company is heading to blockchain development and this project is not an isolated effort. It is a step towards blockchain trading app.
Evolutions in the VeChainThor Stack will be followed up for needed and potential updates.

## Additional Information 

Possible additional information to include:

- What work has been done so far?
The related work is included in the github repositories pointed out in this grant application.

- Are there any teams who have already contributed (financially) to the project?
No.

- Have you applied for other grants so far?
We have not applied for any other grant yet.

# VeChain General Grant Application

## Project Overview

- Project: Whal3s - SaaS token gating platform with SDK
- Team Name: Whal3s GmbH
- Payment Address: [0x469BC30ca7d9F4E85FC3308D1AC93d7922280956](https://etherscan.io/address/0x469BC30ca7d9F4E85FC3308D1AC93d7922280956)

### Overview

The Whal3s token gating framework allows any web2 developer to integrate NFT technology into websites, apps, and games - to build connected / "interoperable" brand experiences within e-commerce, content platforms and in real life.

To reduce the development time from a few months to a few minutes Whal3s offers

1.  Whal3s SDK: Similar to the Stripe SDK, it enables developers to incorporate token-based experiences into any app or website i.e. access control
2.  Whal3s UI components: Similar to the Stripe checkout page, it facilitates the process of users claiming utility from their tokens. ([https://www.youtube.com/watch?v=w7SIqmxJZiw](https://www.youtube.com/watch?v=w7SIqmxJZiw)) test out here: [https://whal3s.xyz/demo](https://whal3s.xyz/demo)
3.  Whal3s App - Analytics and utility dashboard: Provides insights into user engagement, on chain activity and utility consumption.

We apply to this grant to implement VIP-181 tokens to the Whal3s ecosystem.

### Project Details

We are currently live with Ethereum and Polygon and are now looking to become, the leading provider of token gated experiences on Vechain.

- Homepage: [whal3s.xyz](https://whal3s.xyz)
- Demo: [whal3s.xyz/demo](https://whal3s.xyz/demo) (Scroll down)
- Documentation of SDK and API: [docs.whal3s.xyz](https://docs.whal3s.xyz)
- Whal3s App: [app.whal3s.xyz](https://app.whal3s.xyz)
- Github: [github.com/Whal3s-xyz](https://github.com/Whal3s-xyz)
- SDK and React library: [npmjs.com](https://www.npmjs.com/search?q=%40whal3s)


### Ecosystem Fit
We could not find a project in the Vechain ecosystem yet that offers a similar solution. We believe that the Whal3s SDK and UI components will be a great addition to the Vechain ecosystem and will help to onboard more developers and users to the Vechain blockchain.

## Team

### Team members

- Project leader: Jonas Esser (CTO)
- Team Members:
    - Luca Post (CEO)
    - Florian Zeise (COO)

### Team Website

- [https://www.whal3s.xyz](https://www.whal3s.xyz)

### Team's experience

The product is already live for Ethereum and Polygon and in use with various customers. So we already have a lot of experience in framework building as well as in interacting with smart contracts and handling NFTs.
### Team Code Repos

- [github.com/Whal3s-xyz](https://github.com/Whal3s-xyz)

### Team LinkedIn Profiles

- [https://www.linkedin.com/in/luca-post-546508127/](https://www.linkedin.com/in/luca-post-546508127/)
- [https://www.linkedin.com/in/florian-zeise-27786715b/](https://www.linkedin.com/in/florian-zeise-27786715b/)
- [https://www.linkedin.com/in/jonas-esser/](https://www.linkedin.com/in/jonas-esser/)


## Development Roadmap

### Implement Vechain Network to Whal3s Validation Engine

-   The validation engine is an open source, stateless and serverless runtime, that validates a wallet based on the holding NFTs with respect to the requested token gate.
-   Once finished you will be able to run your own validation engine as a node script (e.g. as AWS Lambda) or use the hosted one by Whal3s. This validation engine will be able to check if a users(wallet) matches the conditions of a token gate (for VIP-181 tokens) and has the right signature. E.g. Wallet 0x123…abc owns 1 NFT with a golden background of Collection XYZ on the Vechain Network that is not used yet.
-   Persons involved:
    -   Developers:
        -   Jonas Esser (CTO of Whal3s)
        -   External freelancer
-   Required funding: 14.000€
-   ETA: 01.09.2023-01.10.2023 → 1 Month

### Implement Vechain Network to Whal3s App + API

-   The Whal3s app is the primary interface used (besides the API) to create token gates (utilities). The creator is guided through the process and receives help at many points, e.g. auto-completion to select smart contracts.
-   Once finished you will be able to create token gates with no-code through the Whal3s App or via simple API request
-   Persons involved:
    -   Developers:
        -   Jonas Esser (CTO of Whal3s)
    -   UX/UI
        -   External agency
-   Required funding: 8.000€
-   ETA: 15.09.2023-08.10.2023 → 3 weeks

### Implement Vechain Network to Whal3s SDK

-   The Whal3s SDK includes all the tools needed to implement created token gates into an existing environment (web app, website, mobile app, ...), including React UI components (Modal, Connect Wallet Button, ...).
-   Once finished the Whal3s SDK will fully support Vechain Network. You will be able to use token gates for the Vechain Network. Including functionalities like adding network to wallet, switching network, communication with network, …
-   Persons involved:
    -   Developers:
        -   Jonas Esser (CTO of Whal3s)
        -   External agency
-   Required funding: 7.000€
-   ETA: 15.09.2023-08.10.2023 → 3 weeks


### Total Budget Requested

| Milestone # | Description                                            | Completion Time | Funding  |
|:-----------:|--------------------------------------------------------|-----------------|----------|
| 1           | Implement Vechain Network to Whal3s Validation Engine | 30 days         | 14.000 € |
| 2           | Implement Vechain Network to Whal3s App + API         | 21 days         | 8.000 €  |
| 3           | Implement Vechain Network to Whal3s SDK               | 21 days         | 7.000 €  |


**Total budget request: 29.000€**

#### Community engagement

To publicize and promote the new feature, we will…
- write guides on how to use and host the validation engine
- update the documentation on how to utilise Vechain Network NFTs with Whal3s (App, API and SDK)
- create a YouTube tutorial that developers follow along to build their own token gated application in under an hour
- write two marketing articles on [medium](https://medium.com/@whal3s) and start a twitter series on how to write token gated applications with Vechain

## Future Plans

With Whal3s, we have laid the foundation for token gated infrastructure. In the future we will focus on developing it into an open source protocol to establish a standard for token gated utility. But also the area of usability must not be neglected. Together with our customers we want to extend the value chain by minting and analytics. Also the lowering of hurdles for Web3 foreign users is an important inventory. We will make onboarding as easy as possible to make NFTs and token gates tangible for the mainstream.

## Additional Information

-   We were part of the Outlier Ventures IPFS Base Camp accelerator program
-   Please contact jonas@whal3s.xyz (Jonas Esser) to discuss the grant agreement and next steps


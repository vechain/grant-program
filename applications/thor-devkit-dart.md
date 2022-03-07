# VeChain General Grant Application thor-devkit.dart

## Project Overview 

- Project: thor-devkit.dart
- Team Name: SayNode Operations AG
- Payment Address: 0x989A38EDEbd2Bd80d4949a9F7462C93FA8055876

### Overview

Flutter is an open source framework by Google for building beautiful, natively compiled, multi-platform applications from a single codebase. At the moment there are SDKs to interact with VeChain using many different languages. Sadly Dart, the language used to create Flutter applications, is not one of them. 

We want to expand the options for developers to interact with the VeChain blockchain and make it as easy as possible for them to use tools with which they are already familiar. Our team created Flutter apps in the past and recently published the first Flutter app with a VeChain integration. Since there is no Dart SDK this was a relatively difficult process. To streamline this process for Flutter developers in the future we want to build a VeChain Dart SDK. The unique features of VeChain make it our blockchain of choice and if we can create tools to make its use easier that would be great. 

### Project Details

Our goal is to create a dart SDK that provides the same features and functionalities of the other VeChain SDKs. 
We want to provide the options to use: 
- Public key, private key, address conversion.
- Mnemonic Wallets.
- HD Wallet.
- Keystore.
- Various Hashing functions.
- Signing messages.
- Verify signature of messages.
- Bloom filter.
- Transaction Assembling (Multi-task Transaction, MTT).
- Fee Delegation Transaction (VIP-191).
- Self-signed Certificate (VIP-192).
- ABI decoding of "functions" and "events" in logs.

The end product is a dart package that is public and accessible on https://pub.dev/ for anyone to use.
We worked to integrate VeChain using Dart in our prior app Tree for two: https://github.com/SayNode/342

### Ecosystem Fit

Currently there are no other working dart packages for VeChain and developers have to interact with a node directly or use other languages.

## Team 

### Team members

- Renato Schär
- Werner Liechti
- Yann Marti

### Team Website

- https://saynode.ch/

### Team's experience

- The entire team has a background in computer science from various Swiss universities. Further the team members have a background in development from prior jobs. Our first complete flutter application can be found here: https://github.com/SayNode/342 and has been accepted by both the Apple and Android store. Our team is also performing the token migration of the Dohrnii foundation https://dohrnii.io/ from Ethereum to VeChain and made some related commits.

### Team Code Repos

- https://github.com/SayNode  A few repositories are private because of confidentiality agreements
- https://github.com/RsTs23
- https://github.com/wernerliechti
- https://github.com/Dohrnii-Foundation

### Team LinkedIn Profiles

- https://www.linkedin.com/in/renato-sch%C3%A4r-8a9a19a5/
- https://www.linkedin.com/in/werner-liechti-568b19213/

## Development Roadmap 

### Roadmap for the package creation

#### Overview

|  | Milestone 1 | Milestone 2 | Milestone 3 |  Total |
| - | - | - | - | - |
| Estimated Duration | 30 d | 30 d | 30 d | 90 d |
| Full-time equivalent (FTE) | 1.5 | 1.5 | 1.5 | 4.5 |
| Cost (up to $ 30,000) | $ 8,000 | $ 8,000 | $ 8,000| $ 24,000|

#### Milestone 1 — Keys, wallets and utils functionality

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | GNU Lesser General Public License v3.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial. |
| 0c. | Testing Guide | The code will have proper unit-test coverage (90%) to ensure functionality and robustness. In the guide, we will describe how to run these tests |
| 1 | Public key, private key and address conversion | We will develop the functionalities of the SDK for the public key, private key and address conversions. |
| 2 | Mnemonic wallets | We will develop the functionalities of the SDK for the Mnemonic wallets. |
| 3 | HD wallets | We will develop the functionalities of the SDK for the HD wallets. |
| 4 | Keystore | We will develop the functionalities of the SDK for the keystore. |
| 5 | Various hashing functions | We will develop the functionalities of the SDK for the various hashing functions. |


#### Milestone 2  —  Signatures, ABI and transactions

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | GNU Lesser General Public License v3.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial. |
| 0c. | Testing Guide | The code will have proper unit-test coverage (90%) to ensure functionality and robustness. In the guide, we will describe how to run these tests |
| 1 | Bloom filter | We will develop the functionalities of the SDK for the bloom filter. |
| 2 | Signing messages | We will develop the functionalities of the SDK for signing messages. |
| 3 | Verify signature of messages | We will develop the functionalities of the SDK for verifying signature of messages. |
| 4 | Transaction Assembling | We will develop the functionalities of the SDK for the transaction assembling. |
| 5 | ABI decoding of "functions" and "events" in logs | We will develop the functionalities of the SDK for the ABI decoding of "functions" and "events" in logs.|


#### Milestone 3  —  MPP, VIP-191, VIP-192

| Number | Deliverable | Specification |
|-|-|-|
| 0a.| License | GNU Lesser General Public License v3.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial. |
| 0c. | Testing Guide | The code will have proper unit-test coverage (90%) to ensure functionality and robustness. In the guide, we will describe how to run these tests |
| 1 | Multi-task Transaction, MTT | We will develop the functionalities of the SDK for the multi-task transactions.|
| 2 | Fee Delegation Transaction (VIP-191) | We will develop the functionalities of the SDK for fee delegation transaction (VIP-191). |
| 3 | Self-signed Certificate (VIP-192). | We will develop the functionalities of the SDK for self-signed certificates (VIP-192). |

#### Community engagement

We will publish an article on our work on medium. We will provide frequent updates on social media about our current development activities and progress. Once we are done, we will publish an article providing an example of how to use the SDK.

## Future Plans

Our intention is to use the combination of VeChain and Flutter to create many different applications for varying customers in different sectors. By using VeChains unique features like fee delegation we want to create blockchain applications that provide the end user a seamless experience. To do that an easier way to develop will be very helpful

## Additional Information 

- What work has been done so far?
We used some functionalities in our previous app but haven't put them in a well organized package.
- Are there any teams who have already contributed (financially) to the project?
We are currently in the process of founding our company in Switzerland but have not received any financial support outside of our work so far. 
- Have you applied for other grants so far?
No.

# 🌌 Ternoa Fundamentals 

Your one stop shop for everything {Ternoa centric}. Here we cover all aspects of Ternoa and its ecosystem in detail for our users and developers. This doc contains a comprehensive account of everything ranging from Chain Architecture and Security Protocols to Off chain tools. 


[more Introductory content here]


**Note from Anky :** =======================================================================

* `NFT-primitives/Features` under Standby
* Finalizing content for `Blockchain/Chain-Architecture` n `Blockchain/Consensus-Mechanism` I'll add them in afterwards then make small changes.
* Only proofreading and making suggested changes remains after this
====================================================================================

**Table of Contents**

  - Introduction
  - Blockchain
    - Chain Architecture :
      - Security Protocols :
      - Consensus Mechanism :
      - Networks :
  -  NFT Primitives
     - Types :
       - Basic
       - Secret
       - Capsules
       - Soulbound
     - Features:
  - Off Chain (Done)
    - SDK :
      - Introduction
      - Development
    - Indexer :
      - Introduction
      - Architecture
      - Deployment

## Introduction :
**Ternoa is a Decentralized, Open source, NFT-centric Layer 1 blockchain that is multi-chain by design and aims to provide a technical stack to build scalable and secure NFTs with native support for advanced features.**

The Idea of ternoa came into existence for the purpose of creating a technology to enable the forever storage of Data while keeping Security and Privacy in mind (only making it accessible to the owner) with built in Inheritence, to pass it through time if needed.

It's a result of four long years of Research and Development paired alongside immense effort put in by the core team. Looking back, we've come a long way as today Ternoa provides Innovative and [somewhat] Ingeneous solutions for a multitude of problems on the Polkadot ecosystem  {OR}  { Ternoa provides Innovative and [somewhat] Ingeneous solutions on the Polkadot ecosystem for a multitude of problems.}

With accordance to our beliefs in Individual Liberty, Ternoa combines the decentralization aspect with native encryption using Trusted execution environment (TEEs), turning NFTs into secure, private Data containers, allowing users to retain "True Ownership" of Digital Data.  

## Blockchain 

### Chain Architecture :
[Finalizing Content]

### Security Protocols : (TEE ?)

By Integrating Storage and Computing protocols, we've designed our network to provide cutting edge decentralized tech for NFTs.

We ensure true ownership of data and assets via decentralization of key encryption management. Ternoa protocol handles Key re-encryption and registeration requests from the Computing protocol

`Ternoa Protocol` : Sealed Secret keys are stored on both the Ternoa and Computing protocols by their enclaves using Trusted Execution Enciornment (TEE) {architecutre}.Only the enclave can claim ownership of the keys at any given point of time.

No individual or entity {even a central one} can access the NFT Encryption Key apart from the current owner. The *EncKey* of the NFT can be wiped after each upload/download.

`Storage Protocol` : Our Storage Layer is a decentralized storage network which can be used to store {secure} encrypted private data if {needed/the need arises}. We currently support Inter Planetary File System (IPFS) and Arweane whereas support for other storage networks on the Polkadot ecosystem such as Crust will be accessible soon.

As Ternoa doesn't support native file storage, the need for a dedicated, decentralized storage {network/layer} became paramount. Ternoa's chain architecture being developed on the Polkadot substrate framework allows interoperability with existing {networks/blockchains}. This allows Data ownership management on decentralized storage networks along with Seamless data storage experience. This approach to storage is the most advantageous in terms of security and resilience. This functionality also opens the doors for a variety of B-to-B and B-to-C use cases. {too much `this` use}

`Computing Protocol`: functions like Key generation, Key agreement and Shamir secret sharing are executed in enclaves to make sure that the Keys are never available to anyone outside of the enclave.

Enclaves are in a nutshell, private regions which have the ability to protect their contents in such a way that they can't be read or saved by any outside processes. This ability of an enclave to protect its environment in such a way is called Trusted Execution Environment (TEE). TEE is essentially Hardware-level privacy with a low runtime overhead {which makes sure it doesn't take a huge computational hit}.

TEEs encrypt the enclaves and then decrypt them on the fly, but only within the cpu, and even then only for code and data running from within the enclave itself. The processor thus protects the code from being spied on or examined by other code.

This capability in today’s processors is called Secure Execution Environment for AMD, Software Guard Extension for Intel and Secure Execution for IBM. 

Certified master nodes on our network will take advantage of the inbuilt capabilities of these processors to establish TEEs. This would in turn sheild the nodes from malicious code. It'll offer a secure area within the processor whih protects both the confidentiallity and Integrity of the Data inside of it which is especially important for zero trust networks like ternoa. We've named them **Secret nodes** due to obvious reasons 😅 . 

### Consensus Mechanism :

Sustainability is One of our Core beliefs, keeping that in mind we ensure state-of-the-art energy consumption by using Nominated Proof of Stake (NPoS) for our protocol.
 
[Finalize content]

### Networks :
The ternoa chain consists of multiple networks with varying use cases. It contains both Mainnets and DevNets. Local blockchain environment or DevNets are being used to test out cutting edge tech dapps by our users and developers alike to test dapps before deployment.

**There are currently two active, public networks on the Ternoa Chain, namely :**

`Mainnet` : The Mainnet is the stable production ready network of the Ternoa ecosystem. As the name suggests, it's where the real transactions/interactions take place. It's where the real exchange of value takes place in the ecosystem. 

The role of the Mainnet is to provide a stable production environment for the interaction and actual deployment of Dapps on the Ternoa Chain alongside enabling transfer of real value. 

Every feature added to this network is rigorously tested beforehand on the Alphanet. Only after that is the functionality officially added to the production version

The security of the network is handled by Ternoa alongside external validators meanwhile the governance is taken care of by democratic means where individuals vote according to their relative power decided by their stake.

`Alphanet` : The Alphanet is a stable pre production enviornment used by Devs and users alike to test out our exciting experimental features or to deploy prototype Dapps and rigourously test out their functionality before deeming them Production [worthy/ready].

It provides a stable testing environment for [development/production] and deployment which resembles the Mainnet closely. 

Any feature headed for the Mainnet is Deployed and tested out thouroughly on the alphanet before being cleared for deployment on the mainnet.

It's configured the same as the Mainnet in all aspects except one, only difference being that it gets the same feature updates earlier than its Production-Ready counterpart.

The security of the network is handled by Ternoa alongside external validators meanwhile the governance is taken care of by democratic means where individuals vote according to their relative power decided by their stake.

To incentivise the security of the Alphanet, one recieves ERC-20 $CAPS for validating the network. 

**Apart from these two, there were two other networks which weren't available publically**

`Testnet` [Obsolete]: The Testnet initially aimed to provide a pre production enviornment for our users and devs to test out cutting edge functionality. However, we've decided to retire this network due to {its obsolecense / a change of plans over time}.

`Chaosnet`: The Chaosnet was created for replacing the Testnet which aimed to provide a pre-production environment meant to be used by our users and devs to test new and existing functionality.

Its role will be to provide a pre production environment that contains the latest changes from the chain repo with the added ability to reset the network multiple times without consequences.

This network will be fully controlled by Ternoa aka no external validators or democratic governance. It's not available for public use yet but we'll update you as sson as anything changes in that regard.

## NFT Primitives 

### Types
#### Basic NFTs
Basic NFT refers to an "Phygital" (amalgation of Physical and Digital) asset which is unique, Immutable and transferrable. These can possess a different value from one another even if they come from the same smart contract.

The best part bieng that the owner of a Basic NFt retains the power to Delegate (or Lend) an NFT to a third party with an option to revoke delegation rights.

Basic NFTs possess inbuilt royalty functionality a.k.a. They are programmed to pay the creator(s) a royalty fee each time the NFT is sold on the secondary market, allowing creators to be rewarded fairly for their work.

Users can mint Images, Videos, Music, Documents and even Binary Blobs with support for all major formats using the Basic NFT which uses the TSP-721 standardization which is similar to ERC-721.

Supported Formats :
JPEG, JPG, PNG, GIF, MP4, MOV

To be Added :
SVG, GLB, GLTF, MP3, WEBM among others

#### Secret NFTs

While the blockchain as a public ledger of transactions provides irrefutable proof of ownership of NFTs, it does not meet the data privacy standards needed for many of the NFT use cases. There are situations where it's important to be able to store information in an encrypted and decentralized manner. Secret NFTs have been designed by Ternoa with this in mind. It is Ternoa's State of the Art feature.

Secret NFTs are a special kind of NFTs as in they support encrypted data. Only the current owner of the secret NFT can decrypt the secret NFT at any point. These can be used to store confidential data, for example- legal deeds, Identification (social security no etc), confidential company details among others.

We provide the highest level of security and privacy to our users which ar at par with the best security standards in the industry. We've integrated Intel’s SGX which is a hardware-based memory encryption and trusted computing technology that isolates specific application code and data in memory to maximize confidentiality. 

Ternoa uses Inter planetary File storage (IPFS) for encrypted data storage. This ensures End-to-End encryption of the secret assosiated with the NFT at the time of minting. This means that the encrypted media is stored on decentralized IPFS nodes and the decryption keys are stored on the SGX nodes (Decentralized Key encryption) which can be anywhere worldwide.

#### Capsules 

Capsules are essentially enhanced NFTs (picture Post serum Steve rogers aka Captain America) which can store encrypted data in its capsulized form. 

Encryption for Secret NFTs work similar to Capsule Encryption i.e. at par with the best security standards in the industry namely We've integrated Intel’s SGX which is a hardware-based memory encryption and trusted computing technology that isolates specific application code and data in memory to maximize confidentiality. 

Ternoa uses Inter planetary File storage (IPFS) for encrypted data storage. This ensures End-to-End encryption of the secret assosiated with the NFT at the time of minting. This means that the encrypted media is stored on decentralized IPFS nodes and the decryption keys are stored on the SGX nodes which can be anywhere worldwide. The Data in the capsule will also be backed up on other decentralized data storage protocols such as Arweave or Storj.

The user can convert their NFT into a capsule and vice versa. However, it results in loss of data in the capsule as set forth by the Transmission Protocol selected at the time of capsulization. 

Transmission of Capsule NFTs are designed to get triggered by time and chronological events happening in one’s life. One thing to note is that the transmission protocols will only be applied to capsulized NFTs and not the regular NFTs. (Time Capsule will not be passed on if it isn't capsulized). Learn more about the Transmission Protocols in the [Features section](inc link).

##### Transmission protocol

We understand the importance of certain moments that can trigger the mood in one’s life. The Ternoa protocols are designed to trigger the transmission of your digital assets at a chosen time. Here are the five decentralized ways to make your digital assets travel through time:

Safe Protocol: The best way to protect your data on the blockchain. This protocol allows you to store data in a decentralized manner through the Ternoa Blockchain, and consult and retrieve it at any time. More media, resync feature, money? Can we put the CAPS?

D-Day Protocol: The D-Day Protocol allows you to send a capsule to the chosen recipients by programming a certain date. On that chosen day, the protocol will be triggered and the recipients will receive the decryption keys to open their capsule.

Countdown Protocol: The perfect rescue protocol. This transmission setting allows you to activate a countdown before sending the capsule. Before the protocol is triggered, a countdown will start (1 month, 1 year, 10 years, etc.). If the capsule is not opened within the allotted time, the capsule is automatically sent to the chosen recipients who can then open it.

Consent Protocol: Gain peace of mind thanks to the Consent Protocol, allowing your trusted ones to request access to your capsule at any time. In the event of no response within the chosen time frame, the protocol will be triggered and your loved ones will be able to access the content of the time capsule.

Death Protocol: Everyone leaves something important behind. The Death Protocol offers the possibility to create a capsule that can only be opened after the creator has passed away. A way to ensure that you pass on everything that is important to you to the right people.

#### SoulBound NFTs

Soulbound Tokens refer to the non transferrable nature of the asset. They are unique and immutable but unlike Basic NFTs, their ownership can't be transferred. The name implying the token is bound to the the wallet's soul. 




Our key primitive is accounts, or wallets, that hold publicly visible, non-transferable (but possibly revocable-by-the-issuer) tokens. We refer to the accounts as “Souls” and tokens held by the accounts as “Soulbound Tokens” (SBTs).

Imagine a world where most participants have Souls that store SBTs corresponding to a series of affiliations, memberships, and credentials. For example, a person might have a Soul that stores SBTs representing educational credentials, employment history, or hashes of their writings or works of art. In their simplest form, these SBTs can be “self-certified,” similar to how we share information about ourselves in our CVs. But the true power of this mechanism emerges when SBTs held by one Soul can be issued—or attested—by other Souls, who are counter-parties to these relationships. These counter-party Souls could be individuals, companies, or institutions. For example, the Ethereum Foundation could be a Soul that issues SBTs to Souls who attended a developer conference. A university could be a Soul that issues SBTs to graduates. A stadium could be a Soul that issues SBTs to longtime Manchester United fans.


Furthermore, the lack a native web3 identity makes today’s DeFi ecosystem unable to support activities ubiquitous in the real economy, such as undercollateralized lending or simple contracts, like an apartment lease. In this paper, we illustrate how even small and incremental steps towards representing social identity with soulbound tokens could overcome these limitations and bring the ecosystem far closer to regenerating markets with their underpinning human relationships in a native web3 context. 

Let’s understand how native web3 social identity, with rich social composability, could yield great progress on broader long-standing problems in web3 around wealth concentration and vulnerability of governance to financial attacks, while spurring a Cambrian explosion of innovative political, economic, and social applications. We refer to these use cases as “Decentralized Society” (DeSoc).

## Off Chain

### Ternoa SDK
#### Introduction
It's the easiest and fastest way to build on top of the Ternoa Chain. Based on Javascript and the Polkadot.js API, it offers developers a seamless experience in the Domain of Web 3. 

We aim to provide developers with the technical stack and all the tools and guides nessesary for building scalable and secure NFTs with native support for advanced features.

As Ternoa-js is an open-source SDK, feel free to interact with the tools and libraries, log issues, create pull requests or leave feedback. We welcome and greatly appreciate your contribution.Check out our [Contribution Guidelines](https://github.com/capsule-corp-ternoa/ternoa-js/blob/main/CONTRIBUTING.md) if you wish to do so.

#### Development
If you want to learn how to use the Ternoa SDK, the [test-dapp](https://github.com/capsule-corp-ternoa/ternoa-js-test-dapp) is the perfect place to familiarize yourself with our architecture and contribute to its development.

If you want to start building on the Ternoa ecosystem, [start here](https://github.com/capsule-corp-ternoa/ternoa-js/tree/dev).

### Indexer 
#### Introduction
The Indexer is used to transform blockchain data into a queryable GraphQL database.

A Blockchain stores data in a very disperesed manner, making it incredibly streneous to query relevant data for a specific usecase. There isn't a native feature/functionality to Identify, sort and query linked data (spanning across multiple blocks).

That's where the Indexer comes into play, it scans through each block and records all of the transactions. It then parses all of that data into entities and inserts it into a postgres database. 

Thus allowing one to leverage relevant data according to their specific search filters in a simplified manner.

Ternoa deploys its own indexer, however one can run their own if needed.

#### Architecture
The Indexer goes block by block and parses all the data into a managed Postgress Database.
(Insert pic)
It's composed of a GraphQL API alongside a Worker which handles the Indexing. This Duo is hosted on an Ubuntu Virtual Machine.

The Indexer is currently hosted on a single VM. It'll later be upscaled to version with 'n' number of Indexer APIs and Indexer Workers hosted across multiple VMs with Load balancers to optimize the entire process.
(Insert pic target arch)

(crosscheck if one VM can only run 1 API and 1 worker or...?)

#### Deployment
Deployment of the Indexer on a Virtual Machine requires the installation and set up of NodeJS to buld and run the implementation, and a Postgres Database to store the indexed Data.

Learn more about [Ternoa's Indexer](https://github.com/capsule-corp-ternoa/ternoa-subql) over at the Github Repository.
# Ternoa Fundamentals 

## Introduction :

**Ternoa is a Decentralized, Open source, NFT-centric Layer 1 blockchain that is multi-chain by design and aims to provide a technical stack to build scalable and secure NFTs with native support for advanced features.**

The Idea of ternoa came into existence for the purpose of creating a technology to enable the forever storage of Data while keeping Security and Privacy in mind (only making it accessible to the owner) with built in Inheritence, to pass it through time if needed.

It's a result of four long years of Research and Development paired alongside immense effort put in by the core team. Looking back, we've come a long way as today Ternoa provides Innovative and [somewhat] Ingeneous solutions for a multitude of problems on the Polkadot ecosystem  {OR}  { Ternoa provides Innovative and [somewhat] Ingeneous solutions on the Polkadot ecosystem for a multitude of problems.}

With accordance to our beliefs in Individual Liberty, Ternoa combines the decentralization aspect with native encryption using Trusted execution environment (TEEs), turning NFTs into secure, private Data containers, allowing users to retain "True Ownership" of Digital Data.

## Blockchain 

### Chain Architecture :

[Regular stuff first them come to the more specialized stuff ] (couldn't find/didn't have access to relevent documentation)

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

`Explain Nominated Proof Of Stake`


PoS incentivices honest behaviour and vice versa


### On Chain Transactions : [On Standby]


### Tokenomics and Token Distribution :


### Security :


### Governance :


###  Networks :

There are currently two active, public networks on the Ternoa Chain, namely :

`Mainnet` : The Mainnet is the stable production ready network of the Ternoa ecosystem. As the name suggests, it's where the real transactions/interactions take place. It's where the real exchange of value takes place in the ecosystem. 

The role of the Mainnet is to provide a stable production environment for the interaction and actual deployment of Dapps on the Ternoa Chain alongside enabling transfer of real value. 

Every feature added to this network is rigorously tested beforehand on the Alphanet. Only after that is the functionality officially added to the production version

The security of the network is handled by Ternoa alongside external validators meanwhile the governance is taken care of by democratic means where individuals vote according to their relative power decided by their stake.

`Alphanet` : The Alphanet is a stable pre production enviornment used by Devs and users alike to test out our exciting experimental features or to deploy prototype Dapps and rigourously test out their functionality before deeming them Production [worthy/ready].

It provides a stable testing environment for [development/production] and deployment which resembles the Mainnet closely. 

Any feature headed for the Mainnet is Deployed and tested out thouroughly on the alphanet before being cleared for [.....]

It's configured the same as the Mainnet in all aspects except one, only difference being that it gets the same feature updates earlier than its Production-Ready counterpart.

The security of the network is handled by Ternoa alongside external validators meanwhile the governance is taken care of by democratic means where individuals vote according to their relative power decided by their stake.

To incentivise the security of the Alphanet, one recieves ERC-20 $CAPS for validating the network. 

**Apart from these two, there were two other networks which weren't available publically**

`Testnet` [Obsolete]: The Testnet initially aimed to provide a pre production enviornment for our users and devs to test out cutting edge functionality. However, we've decided to retire this network due to {its obsolecense / a change of plans over time}.

`Chaosnet`: The Chaosnet was created for replacing the Testnet which aimed to provide a pre-production environment meant to be used by our users and devs to test new and existing functionality.

Its role will be to provide a pre production environment that contains the latest changes from the chain repo with the added ability to reset the network multiple times without consequences.

This network will be fully controlled by Ternoa aka no external validators or democratic governance. It's not available for public use yet but we'll update you as sson as anything changes in that regard.


### Staking :

Staking with the Ternoa ecosystem helps with improving network security 

### Nodes :
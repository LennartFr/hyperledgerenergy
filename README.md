# Blockchain product overview
<p>
<img src="https://www.hyperledger.org/wp-content/uploads/2016/09/logo_hl_new.png"><p>
<p>
[Hyperledger](https://www.hyperledger.org/) is an umbrella project of open source blockchains and related tools, started in December 2015 by the Linux Foundation, to support the collaborative development of blockchain-based distributed ledgers.
<p>

[Hyperledger Fabric](github.com/hyperledger/fabric) is an implementation of a distributed ledger platform for running smart contracts, leveraging familiar and proven technologies,  with  a  modular  architecture  allowing  pluggable  implementations  of  various  functions.
<p>
<p>
<img src="https://farm5.staticflickr.com/4630/27933522299_0f031eb17b_o.jpg" width="638" height="359" alt="Hyperledger">
<p>

## The Blockchain Distributed Ledger
<img src="https://www.ibm.com/blogs/internet-of-things/wp-content/uploads/2017/05/2-1.jpg">
<p>

[Hyperledger Composer](https://www.hyperledger.org/projects/composer) Hyperledger Composer is a set of collaboration tools for building blockchain business networks that make it simple and fast for business owners and developers to create smart contracts and blockchain applications to solve business problems.
<p>

# Designing and creating Blockchain applications with Hyperledger
[IBM Design Thinking Field Guide](https://www.ibm.com/blogs/bluemix/2016/12/ibm-design-thinking-field-guide/)

# Blockchain Use Cases
[IBM Blockchain Use cases](https://www.ibm.com/blockchain/use-cases/)

# IBM Blockchain course
[Zero to Blockchain An IBM Redbooks course by Bob Dill, David Smit] (shttps://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/crse0401.html])



<img src="https://farm5.staticflickr.com/4458/37771305586_6bf75bc2af_o.png" width="853" height="482" alt="hyperledger architecture">  
<p>

## Blockchain main components 

### Ordering Service – Ordering and synchronizing transactions
... the ordering service is the definition of the network. It contains identity information for each member, information on channels and a set of policies dictating which members are permitted to perform certain tasks (e.g. invite other members, create channels, etc.). Every transaction and configuration operation will flow through the ordering service, so it’s a beyond critical piece in the overall scheme of things.......

#### Consensus
Consensus is the process by which a network of nodes provides a guaranteed ordering of transactions and validates the block of transactions. Consensus must provide the following core functionality:
• 
Confirms the correctness of all transactions in a proposed block, according to endorsement and consensus policies.
• 
Agrees on order and correctness and hence on results of execution (implies agreement on global state).
• 
Interfaces and depends on smart-contract layer to verify correctness of an ordered set of transactions in a block
<p>
Consensus Algorithm: <a href="https://www.hyperledger.org/wp-content/uploads/2017/08/HyperLedger_Arch_WG_Paper_1_Consensus.pdf">Kafka</a>

###  Certificate Authority – Issuing certificates to participants
To put it simply, the Certificate Authority (CA) provides membership. All entities in the network (peers, orderers, clients, etc.) must have an identity to communicate, authenticate and ultimately transact. These “identities” exist in the form of x509 certificates (i.e. enrollment certificates), which are required for any direct participation in the blockchain network.... 

###  Peer – Validating/endorsing transactions
The peer exists to perform two main functions: execute/validate transactions & maintain ledgers. The peer runs smart contracts, and is the holder of transaction history and the current state of assets on the network’s channels. At the end of the day it’s all about accessing the peer (directly or indirectly) and performing reads and writes against the ledger. When a member provides an end user access to the network, they’re really providing access to the functionality of the peer.
<br>
https://console.bluemix.net/docs/services/blockchain/index.html#ibm-blockchain-platform

<img src="https://farm5.staticflickr.com/4523/38243385192_43d682cf94_o.png" width="910" height="483" alt="Hyperledger helloworld 2">
<p>
Chaincode written in Go or Java
<p>
<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

# Blockchain Usecases
[Blockchain usecases from IBM](https://www.ibm.com/blockchain/use-cases/)

# Blockchain Developer Patterns

[Decentralized Energy](https://developer.ibm.com/code/patterns/decentralized-energy-hyperledger-composer/)

[Create your first blockchain network using Hyperledger Composer](https://github.com/IBM/BlockchainNetwork-CompositeJourney?cm_sp=IBMCode-_-build-a-blockchain-network-_-Get-the-Code)

[Deploy an asset-transfer app using blockchain ](https://github.com/IBM-Blockchain/marbles?cm_sp=IBMCode-_-deploy-an-asset-transfer-app-using-blockchain-_-Get-the-Code)

[Blockchain Developer Patterns](https://developer.ibm.com/code/technologies/blockchain/)

<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

# Development with Hyperledger Composer, Hyperledger Fabric and the IBM Cloud

## Step 1: In Composer, develop and run your business network datamodel. Export .bna file
## Step 2: Develop and run your Angular + .bna file + Fabric app locally
## Step 3: Deploy your app to the IBM Blockchain Platform on the IBM Cloud.

# How did it all start?
 
October 2008 It all started with Satoshi Nakamoto and his paper [Bitcoin: A Peer-to-Peer Electronic Cash System](https://bitcoin.org/bitcoin.pdf) which addressed a key problem in electronic commerce:

<img src="https://farm5.staticflickr.com/4505/24079519258_ab8a80f7ed_o.png" width="769" height="229" alt="Double Spending">
<p>
<i>
The first work on a cryptographically secured chain of blocks was described in 1991 by Stuart Haber and W. Scott Stornetta.[17] In 1992, Bayer, Haber and Stornetta incorporated Merkle trees to the design, which improved its efficiency by allowing several documents to be collected into one block.
  </i><p><i>
A blockchain database is managed autonomously using a peer-to-peer network and a distributed timestamping server. The first blockchain was conceptualised by an anonymous person or group known as Satoshi Nakamoto in 2008. 
</i><p>
https://en.wikipedia.org/wiki/Blockchain
<p>
<i>A blockchain is a decentralized virtual ledger for recording transactions without central authority through a distributed cryptographic protocol. It is made up of three technologies 

1. cryptographic algorithms, 
1. a distributed protocol, 
1. and replicated data 
<p>
which combined provide a trustworthy service to a group of nodes that do not fully trust each other. 
<p>
With blockchain, several users can write entries into a block or a record of information, and a community can control how the record of information is modified and updated.
</i>
Consensus protocol is pluggable, currently an implementation of Byzantine fault-tolerant consensus using the PBFT (Practical Byzantine Fault Tolerance) protocol.
<p>
Christian Cachin <a href="https://www.ibm.com/blogs/research/2017/10/resilient-consensus-protocols-blockchains/">Resilient Consensus Protocols for Blockchains</a>
<p>
Source: https://www.zurich.ibm.com/dccl/papers/cachin_dccl.pdf
   

# Resources
## Zero to Bockchain
<a href="https://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/crse0401.html">Zero to Blockchain</a>

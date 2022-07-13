# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

(When user logs in to Metamask using the accout used to deploy the smart contract, this admin ui will be visible. Add farmer, distributon, retailer and consumer using this admin ui. Then for each role, switch the Metamask account to conduct the functionalities for that role.)
![truffle test](images/ftc_admin_ui.png)

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

## Contract on Ropsten

https://ropsten.etherscan.io/address/0x74F91C26929d9A24Cc08687c17A2e3FBcd8b926d

## Project write-up (UML)

### Activity Diagram

![Activity Diagram](images/udacity-nd-bc-activity-diagram.png)

### Sequence Diagram

![Sequence Diagram](images/udacity-nd-bc-sequence-diagram.png)

### State Diagram

![State Diagram](images/udacity-nd-bc-state-diagram.png)

### Class Diagram

![Class Diagram](images/udacity-nd-bc-class-diagram.png)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

Tools version used to compile this project on my machine
|Tool|Version|
|----|-------|
| Truffle | v5.1.14-nodeLTS.0 (core: 5.1.13) |
| Solidity | v0.5.16 (solc-js) |
| Solidity compiler | 0.4.24 |
| Node | v16.13.2 |
| web3.min.js | https://cdn.jsdelivr.net/npm/web3@latest/dist/web3.min.js |
| truffle-contract.js | https://cdn.jsdelivr.net/npm/@truffle/contract@4.3.5/dist/truffle-contract.js |

### Installing

> The starter code is written for **Solidity v0.4.24**. At the time of writing, the current Truffle v5 comes with Solidity v0.5 that requires function _mutability_ and _visibility_ to be specified (please refer to Solidity [documentation](https://docs.soliditylang.org/en/v0.5.0/050-breaking-changes.html) for more details). To use this starter code, please run `npm i -g truffle@4.1.14` to install Truffle v4 with Solidity v0.4.24.

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/udacity/nd1309/tree/master/course-5/project-6
```

Change directory to `project-6` folder and install all requisite npm packages (as listed in `package.json`):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder `build\contracts`.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

## Built With

- [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
- [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
  to make the web faster, safer, and more open.
- [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.

## Authors

See also the list of [contributors](https://github.com/your/project/contributors.md) who participated in this project.

## Acknowledgments

- Solidity
- Ganache-cli
- Truffle
- IPFS

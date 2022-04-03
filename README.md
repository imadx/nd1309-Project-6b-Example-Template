# Sample contracts and transactions on Etherscan

## Contracts

- [FarmerRole: 0xfff2894336e05467ee50aa2dcb4f5cc12a6ebc0f](https://rinkeby.etherscan.io/address/0xfff2894336e05467ee50aa2dcb4f5cc12a6ebc0f#events)
- [DistributorRole: 0x11eed5ccf62d3c4a770f08999432cbfd9871ad91](https://rinkeby.etherscan.io/address/0x11eed5ccf62d3c4a770f08999432cbfd9871ad91#events)
- [RetailerRole: 0x9e2ed19125420944a8797c4fa952a502cc494b00](https://rinkeby.etherscan.io/address/0x9e2ed19125420944a8797c4fa952a502cc494b00#events)
- [ConsumerRole: 0x29a1c2d658aeb7a5f5f1b568e58a666fcf2a6495](https://rinkeby.etherscan.io/address/0x29a1c2d658aeb7a5f5f1b568e58a666fcf2a6495#events)
- [SupplyChain: 0x8d9575a58217f0805dc930c9f1b4a8a41aadc0e3](https://rinkeby.etherscan.io/address/0x8d9575a58217f0805dc930c9f1b4a8a41aadc0e3#events)

## Transactions

- [Harvested: 0xa27c82ba4d42340558253c1a0f79141f03d8b3e090266a85e7d36710262513c5](https://rinkeby.etherscan.io/tx/0xa27c82ba4d42340558253c1a0f79141f03d8b3e090266a85e7d36710262513c5)
- [Processed: 0x3d406f0ec78d7a89fb6eb2e411abb0714fa144e073625149eeeb4cad2179cf3d](https://rinkeby.etherscan.io/tx/0x3d406f0ec78d7a89fb6eb2e411abb0714fa144e073625149eeeb4cad2179cf3d)
- [Packed: 0x1b78608361c409c6c206d783db9d1b26365689c7c278d04f9e769db33ad7c854](https://rinkeby.etherscan.io/tx/0x1b78608361c409c6c206d783db9d1b26365689c7c278d04f9e769db33ad7c854)
- [ForSale: 0x4c69c20dda840627dcbb7e60f45af3c6ee6f9ff7bd1dd5a952098a2c632905d3](https://rinkeby.etherscan.io/tx/0x4c69c20dda840627dcbb7e60f45af3c6ee6f9ff7bd1dd5a952098a2c632905d3)
- [Sold: 0x76456be6303c1d0b100aa9f7729725990848a26f759fe7e7ea28d537d0724b85](https://rinkeby.etherscan.io/tx/0x76456be6303c1d0b100aa9f7729725990848a26f759fe7e7ea28d537d0724b85)
- [Shipped: 0x48313928aa6f14ad838f5008a5d5b92d25b0b58ed04c5083684ee68cf264a497](https://rinkeby.etherscan.io/tx/0x48313928aa6f14ad838f5008a5d5b92d25b0b58ed04c5083684ee68cf264a497)
- [Received: 0x6a51ed830605a332b84da41573916e205715212e916fa9f51ecae5bd70aa5696](https://rinkeby.etherscan.io/tx/0x6a51ed830605a332b84da41573916e205715212e916fa9f51ecae5bd70aa5696)
- [Purchased: 0xb961badf46d11dbce4f20043d73b47d3f86b96420428c502f816532bb71bdaa8](https://rinkeby.etherscan.io/tx/0xb961badf46d11dbce4f20043d73b47d3f86b96420428c502f816532bb71bdaa8)

# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)
```

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

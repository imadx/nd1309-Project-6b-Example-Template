# Sample contracts and transactions on Etherscan

## Contracts

- [FarmerRole: 0xf6831f19858c606a3e3c6ea8a3897d2e74ddca86](https://rinkeby.etherscan.io/address/0xf6831f19858c606a3e3c6ea8a3897d2e74ddca86#events)
- [DistributorRole: 0xe6664d627104422dc320e1fe626c8e5ad5545f24](https://rinkeby.etherscan.io/address/0xe6664d627104422dc320e1fe626c8e5ad5545f24#events)
- [RetailerRole: 0x3008a950785bdd85a4fda07872ecde3127acd40e](https://rinkeby.etherscan.io/address/0x3008a950785bdd85a4fda07872ecde3127acd40e#events)
- [ConsumerRole: 0x54a05d75d1bdc3144f432b364dfa625e27a23bfd](https://rinkeby.etherscan.io/address/0x54a05d75d1bdc3144f432b364dfa625e27a23bfd#events)
- [SupplyChain: 0x26cb51178547802ee8007f5f746631946206f70f](https://rinkeby.etherscan.io/address/0x26cb51178547802ee8007f5f746631946206f70f#events)

## Transactions

- [Harvested: 0x7dab5c97274a166ff3e0477e45d5911aec6a7dbb6b97b25dc69e660e6eff22b4](https://rinkeby.etherscan.io/tx/0x7dab5c97274a166ff3e0477e45d5911aec6a7dbb6b97b25dc69e660e6eff22b4)
- [Processed: 0x985443843164255f1624169ddd7d5b0a1baa8baf7ce711b4a7406f468c106889](https://rinkeby.etherscan.io/tx/0x985443843164255f1624169ddd7d5b0a1baa8baf7ce711b4a7406f468c106889)
- [Packed: 0x7f44fd8d328438ea7374a85a79c4d7dc52dff02f6f38c807d025aed41e309bdf](https://rinkeby.etherscan.io/tx/0x7f44fd8d328438ea7374a85a79c4d7dc52dff02f6f38c807d025aed41e309bdf)
- [ForSale: 0x311fda5d610947b3b428ed0bd23e9468209b32fcc718c16476f06fd1308d4037](https://rinkeby.etherscan.io/tx/0x311fda5d610947b3b428ed0bd23e9468209b32fcc718c16476f06fd1308d4037)
- [Sold: 0xd2193fa49aa4125ad31597a5bff6ccc9904beb7cb4360fc281ab2462d232e467](https://rinkeby.etherscan.io/tx/0xd2193fa49aa4125ad31597a5bff6ccc9904beb7cb4360fc281ab2462d232e467)
- [Shipped: 0x61c318d1e8e976c3445cacfada8ea85fe9c86c9f96b66e46f676f18ed7b74b1d](https://rinkeby.etherscan.io/tx/0x61c318d1e8e976c3445cacfada8ea85fe9c86c9f96b66e46f676f18ed7b74b1d)
- [Received: 0xa33866a94dc3cb11615c719a2df705fa970537fb842115eeb88c2f6bafcb9b37](https://rinkeby.etherscan.io/tx/0xa33866a94dc3cb11615c719a2df705fa970537fb842115eeb88c2f6bafcb9b37)
- [Purchased: 0x5f4a24ee7fb43d2b3ae0b32303c2e83330763d244fbe04314fc6a9a0c1affa31](https://rinkeby.etherscan.io/tx/0x5f4a24ee7fb43d2b3ae0b32303c2e83330763d244fbe04314fc6a9a0c1affa31)

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

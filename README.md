# 🏗 Scaffold-ETH 2 powered smart contract portfolio

This repository contains all the implementation contracts of various use cases that I have built or experimented with. Navigate to the different branches to check the contract implementation and play with the contracts using Scaffold Eth UI

Note: All the contracts implemented here are only for learning purposes and might not be production ready.
All the security best practises may or may not be followed due to time constraints.

### (In progress - Many smart contracts are yet to be added soon)

### DeFi

Decentralized Exchange Contract - [Click Here](https://github.com/venkatesh16031999/DEX-Contract-Eth-Scafold-2/tree/defi/dex-smart-contract)

### Upgradable Contracts:

Basic Diamond Proxy Contract (EIP-2535) - [Click Here](https://github.com/venkatesh16031999/Blockchain/tree/upgradable/diamond-proxy-contract) 


### Low level EVM

Assembly -

## Requirements to play with the contracts

Before you begin, you need to install the following tools:

- [Node (v18 LTS)](https://nodejs.org/en/download/)
- Yarn ([v1](https://classic.yarnpkg.com/en/docs/install/) or [v2+](https://yarnpkg.com/getting-started/install))
- [Git](https://git-scm.com/downloads)

## Quickstart

To get started with Scaffold-ETH 2, follow the steps below:

1. Clone this repo & install dependencies

```
git clone https://github.com/scaffold-eth/scaffold-eth-2.git
cd scaffold-eth-2
yarn install
```

2. Run a local network in the first terminal:

```
yarn chain
```

This command starts a local Ethereum network using Hardhat. The network runs on your local machine and can be used for testing and development. You can customize the network configuration in `hardhat.config.ts`.

3. On a second terminal, deploy the test contract:

```
yarn deploy
```

This command deploys a test smart contract to the local network. The contract is located in `packages/hardhat/contracts` and can be modified to suit your needs. The `yarn deploy` command uses the deploy script located in `packages/hardhat/deploy` to deploy the contract to the network. You can also customize the deploy script.

4. On a third terminal, start your NextJS app:

```
yarn start
```

Visit your app on: `http://localhost:3000`. You can interact with your smart contract using the contract component or the example ui in the frontend. You can tweak the app config in `packages/nextjs/scaffold.config.ts`.

Run smart contract test with `yarn hardhat:test`

- Edit your smart contract `YourContract.sol` in `packages/hardhat/contracts`
- Edit your frontend in `packages/nextjs/pages`
- Edit your deployment scripts in `packages/hardhat/deploy`

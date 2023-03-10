# ethereum-gas-tracker
Project for tracking Ethereum gas, allowing to observe gas prices in real time.

## Definitions

**Gas** is a unit that measures the amount of computational effort required to carry out a specific operation on the Ethereum network. In general, the more complex a program (or smart contract is), the more gas it consumes. Since each Ethereum transaction requires computational resources to execute, each transaction requires a fee. Gas refers to the fee required to execute a transaction on Ethereum, regardless of transaction success or failure.

**Gas price** is the amount paid by the deployer (or sender) for each unit of gas. Gas prices tend to fluctuate wildly on public blockchains, especially Ethereum, and the way to compute it has also changed drastically since its inception.

**Gas limit** refers to the maximum amount of gas you are willing to consume on a transaction. More complicated transactions involving smart contracts require more computational work, so they require a higher gas limit than a simple payment. A standard ETH transfer requires a gas limit of 21,000 units of gas.

**Gwei** ``1 gwei = 0.000000001 ETH (10^-9 ETH)``

## Computing gas prices

```units of gas used * (base fee + priority fee)```

- ``units of gas used`` is gas limit.
- ``base fee`` is the value set by the protocol.
- ``priority fee`` is a value set by the user as a tip to the validator.

## How to install it

1. Install NPM and node

```node -v```

2. Sign up for an Infura Account and get API key
3. Rename .env_dev to .env and paste your API key
4. Download repo

```
npm install
npm start
```

5. Visit https://localhost:3000, you should see a web app

## Sources

- [Medium article](https://levelup.gitconnected.com/how-to-build-an-ethereum-gas-tracker-with-infura-42e8ac557441)
- [Ethereum docs](https://ethereum.org/en/developers/docs/gas/)




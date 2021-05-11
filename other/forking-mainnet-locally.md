---
description: >-
  Mainnet forks allow developers to test out contracts and transactions on
  mainnet without actually doing irreversible and costly transactions.
---

# Forking mainnet locally

Clone the Risk Harbor Contracts repo and install dependencies:

```bash
git clone https://github.com/Risk-Harbor/RiskHarbor-Contracts.git
yarn install
```

Start mainnet fork where `<key>` is placed with a AlchemyApi key.

```bash
npx hardhat node --fork https://eth-mainnet.alchemyapi.io/v2/<key>
```

{% hint style="info" %}
If you want to fork mainnet at a specific block: 

```text
npx hardhat node --fork https://eth-mainnet.alchemyapi.io/v2/<key> --fork-block-number <block number>
```
{% endhint %}




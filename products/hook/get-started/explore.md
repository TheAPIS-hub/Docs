---
description: Explore have selected the particular data chart for end user
---

# Explore

* Marketcap comparative change&#x20;
* Trading volume change
* Addresses increment
* Top NFT collections in a day
*   &#x20;Top DeFi projects in a day



![Explore in Hook](<../../../.gitbook/assets/Dashboard (2).png>)

## Everyone’s an Investor

\-Providing Actionable Data to Enable This Future

### Metrics explain

### L1 chain:

$$
Aum=∑ (price*asset)
$$

\
Asset is a database of all ERC-20s, ERC 721s, and ERC 1115s.&#x20;



Revenue: Σ transaction fees per block, for n blocks over time t. Transaction fees = total gas spent \* price of gas. In Ethereum’s case, include the base fee (the base fee is the part of the transaction fee that is burned in each Ethereum block) as part of the transaction fee category.

\
**Ether-Specific Add-ons:**&#x20;

Tokens Burned: Σ base fee per block, for n blocks since the launch of EIP1559 (the Berlin Hardfork (August 5, 2021).&#x20;

Inflation Rate: (block reward – base fee)/supply. Can take a 7 day moving average to calculate/graph the rate more steadily (less volatile).&#x20;

Burn Percentage: base fee/(base fee + tip). Tip is the remainder of the transaction fee, what is actually paid to the miner: total transaction fee = base fee + tip.\


### AMMs:

\
Each protocol below likely has a contract factory for launching of sub-markets: i.e. specific AMM pools, money markets (in the case of lending protocols), and vaults (in the case of yield-aggregating products).&#x20;



Automated Market Maker (AMM) Protocols: AUM: Σ value of LP tokens = Σ Price/asset \* # of that asset, for all assets locked in each sub-market. Each protocol has a contract factory for launching sub-markets, i.e. ETH-USDC pool; ETH-USDT pool; LINK-ETH pool; etc.&#x20;



Revenue (to LPs, not token holders): Σ Transaction Volume \* sub-market fee (each sub-market can have a different transaction fee, although how that is encoded is standardized across each protocol).&#x20;



Edge case alert: Note that depositing into the smart contract as a liquidity provider will almost always be a ‘part-transaction’, where the ratio of the deposit doesn’t match the current AMM ratio precisely, and so a fraction of the assets deposited are traded to ‘re-balance’ the pool.&#x20;



Revenue to token holders = Revenue to LPs \* protocol fee (can be found for each protocol—can assume 0 for now, as all besides Curve are)\


### Lending protocols&#x20;

AUM: Σ assets deposited by lenders (doesn’t include collateral posted by borrowers)&#x20;

Collateral: Σ assets deposited by borrowers Revenue (not sure most feasible way to measure—likely programmed into each smart contract in a way that is standardizable): Σ AUM \* interest paid Revenue to token holders: Revenue to LPs \* protocol fee, if applicable (can assume 0/ignore at the moment) Compound Aave Cream Bucket 3b Stablecoin Protocols (very similar/identical to lending protocols, just issuing a new currency for the loan): AUM: Σ currency outstanding/issued (doesn’t include collateral posted by borrowers), i.e. total Dai in existence in the case of Maker Collateral: Σ assets deposited by borrowers Revenue not sure most feasible way to measure—likely programmed into each smart contract in a way that is standardizable: Σ AUM \* interest paid = Revenue to native token holders (can think of native token holders as the LPs here) Maker Liquity\


### Derivatives Protocols&#x20;

AUM: Σ loans issued (doesn’t include collateral posted by borrowers)&#x20;

Collateral: Σ assets deposited by borrowers Revenue (not sure most feasible way to measure—likely programmed into each smart contract in a way that is standardizable): Σ AUM \* interest paid Revenue to token holders: Revenue to LPs \* protocol fee, if applicable (can assume 0/ignore at the moment) dYdX Synthetix Mirror\


### Yield Aggregating Protocols&#x20;

(most complex for revenue—even the best ones—don’t do revenue for these guys yet):&#x20;

$$
\sum(\text{price} \cdot \text{asset})
$$

AUM: Σ Price/asset \* # of that asset, for all assets locked in each vault. Each protocol has a contract factory for launching vaults, i.e. ETH vault; USDC vault; stETH vault; etc.. Yearn Finance Alpha Homora Convex Rari Bucket&#x20;

### Staking Protocols:&#x20;

AUM: Σ Ether deposited Revenue: Staking reward of their AUM; or AUM \* interest, where interest is the current Eth staking reward Lido Finance&#x20;

### Popular NFT Projects:&#x20;

AUM: 0/NA (not applicable) Revenue: Σ transaction volume \* protocol fee of OpenSea Axie Infinity\
\
\


{% hint style="info" %}
This section is under development, soon will be released. Please us on [social media](../../../get-in-touch/contact-us.md) for the latest information.
{% endhint %}

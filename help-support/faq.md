# General FAQ

This FAQ page answers some of the more commonly asked questions from the PlexSwap community.

## Is PlexSwap safe? Has PlexSwap been Audited?

Although there is still no independent audit report, there are some aspects that you should consider in your assessment:

* We’re built on open-source software: our site and all our Smart Contracts are publicly visible for maximum transparency.
* Our contracts are verified on BscScan so you know that what you see is what you get:\\
  * [Plex Router](https://bscscan.com/address/0x4bAa3F9f24B97aa67B0A0f080bA3A9c994c6AE93#code)
  * [Plex Factory](https://bscscan.com/address/0x580B12Fcc6247E7bA7a02324Ea6Aa6604d0BEC7A#code)
  * [Plex Pair](https://bscscan.com/address/0x539Df50cf6fc29d560413d669A5Bb78cB342029B#code)
  * [Waya Token](https://bscscan.com/address/0x32d9F70F6eF86718A51021ad269522Abf4CFFE49#code)
  * [Chief Farmer](https://bscscan.com/address/0x4D4408eA016357BB334eAd40F14dcF0dfd164Dbe#code)
  * [Crop Chief Factory](https://bscscan.com/address/0xDa804bEC9260C2131a61A2065879AAFc30261f60#code)
  * [Waya Vault](https://bscscan.com/address/0x7899654d3C4f2eEe352c833BD3aBE67Fb18A4D71#code)
  * [Waya Flexible Vault](https://bscscan.com/address/0xB584cA7F7774EB9a68E60C032C45f0Efe9539AFE#code)
  * [Farm Booster](https://bscscan.com/address/0x1A8B1dA52599E31B4BEC6240704F218be001eF84#code)
  * [Farm Booster Proxy Factory](https://bscscan.com/address/0x5D99aAa3838429c242142B8f00152714C88486a5#code)
* Security best practices:
* All Farmers use multisig for all contracts.

## How can I stake WAYA?

You can stake your WAYA in PlexSwap Crop Silos. Visit the [Crop Silos page](https://swap.plexfinance.us/pools).

Read our [How to Stake in Crop Silos guide](https://docs.plexfinance.us/products/crop-silos/crop-silos-guide) if you'd like a hand getting started with staking.

## What is the difference between staking and farming?

Staking in Crop Silos and farming with Yield Farming are both ways to earn more WAYA by supporting PlexSwap.

Staking only needs some WAYA to be added to a Crop Silo to earn WAYA or other tokens.\
[Learn more about Crop Silo staking.](https://docs.plexfinance.us/products/crop-silos)

Farming is more complicated and needs LP Tokens to earn WAYA.\
[Learn more about Yield Farming.](https://docs.plexfinance.us/products/yield-farming)

## How do I farm?

We have a [Yield Farming guide](https://docs.plexfinance.us/products/yield-farming/how-to-use-farms) if you're interested in learning how to farm.

## How do I connect my wallet to BNB Smart Chain and PlexSwap?

We have a [Connect Your Wallet to PlexSwap guide](https://docs.plexfinance.us/plexswap/get-started/connection-guide) covering this in detail.

## What's the best wallet for PlexSwap?

It depends on your needs. We have an [in-depth guide to selecting and creating a wallet](https://docs.plexfinance.us/plexswap/get-started/wallet-guide) that's right for you.

## Why is my transaction failing?

You can check the status of a transaction on [https://bscscan.com/](https://bscscan.com).

Our [Troubleshooting Errors guide](https://docs.plexfinance.us/plexswap/help-support/troubleshooting) may have a solution for your problem if you're having issues.

## When will you open more pools?

New Pools are added to PlexSwap frequently. There will always be an announcement before the launch of new pools.

Join the [announcements Telegram group](https://t.me/PlexSwap) to learn about new Pools as early as possible.

## Did Farm APR calculation change?

Previously, rewards earned by LP Token-holders generated from trading fees were not included in Farm APR calculations. APR calculations now include these rewards, and better reflect the expected APR for Farm pairs.

## How do I get airdrops?

Whenever there is an official airdrop on PlexSwap it will be announced along with the requirements.

Please remember anyone can airdrop tokens to PlexSwap users since every transaction is public on BscScan. Be sure to do your own research when it comes to non-official airdrops. To protect your funds, we recommend you don't use a smart contract you don't understand from a source you don't trust.

## Where can I view smart contracts?

Learn how to find smart contracts on our [Finding Contracts page](https://docs.plexfinance.us/developers/smart-contracts).

## Why does it say I have no BNB balance?

If you've already [transferred BNB into your BNB Smart Chain-enabled wallet](https://docs.plexfinance.us/plexswap/get-started/bep20-guide) but still have this error, you're most likely not [connected to BNB Smart Chain](https://docs.plexfinance.us/plexswap/get-started/connection-guide) within your wallet. Check your wallet's selected network and make sure you have BNB Smart Chain (BSC) selected.

## What is the max supply of WAYA?

$WAYA does not have a maximum supply. The circulating supply is managed through built-in burning and regular burning events.\
\
Read this to [learn more about PlexSwap's tokenomics](https://docs.plexfinance.us/technical-specs/waya/waya-tokenomics).

## What are the treasury funds used for?

The treasury funds are used to cover the expenses involved in running PlexSwap. These expenses include salaries, audits, prizes, hosting, upkeep, bounties, etc.

## Where can I check the Analytics?

You can check the analytics of PlexSwap by click on the "Analytics" tab on the top menu or by clicking the link below.

Analytics: [https://PlexSwap.info/](https://plexswap.info)

## Is PlexSwap protected from flashloan attacks?

PlexSwap's vault has anti-flashloan protection. PlexSwap’s WAYA token isn’t vulnerable to flash loan attacks. Unlike vulnerable tokens, WAYA token minting is predefined, and can’t be adjusted in a single transaction. Ownership cannot be transferred outside of ChiefMaster contract.

PlexSwap’s other smart contracts, like AutoPool, are protected as well; they prevent other contracts from interacting with them, reducing the scope of vector attacks.

## I can't find an answer for my question. Where do I find an answer?

If you can't find what you're looking for in PlexSwap's documentation, ask your question on [PlexSwap's official e-mails](https://docs.plexfinance.us/plexswap/contact-us) and someone will do their best to help you out.

# General FAQ

![](<../.gitbook/assets/general-faq-header (1).png>)

This FAQ page answers some of the more commonly asked questions from the PlexSwap community.

## Is PlexSwap safe? Has PlexSwap been Audited?

See for yourself:

* Check out these PlexSwap security audits:
  * [Certik’s security audit of PlexSwap](https://www.certik.org/projects/PlexSwap) and [Certik's Shield insurance](https://shield.certik.foundation)
  * [Slowmist's security audit of PlexSwap](https://github.com/slowmist/Knowledge-Base/blob/master/open-report/Smart%20Contract%20Security%20Audit%20Report%20%20-%20PlexSwap.pdf)
  * [Slowmist's Auto-WAYA Pool security audit](https://github.com/slowmist/Knowledge-Base/blob/master/open-report/Smart%20Contract%20Security%20Audit%20Report%20-%20WayaVault.pdf)
  * [Peckshield's Lottery V2 Audit](https://github.com/peckshield/publications/blob/master/audit\_reports/PeckShield-Audit-Report-PlexSwapLottery-v1.0.pdf)
  * [Slowmist's Lottery V2 Audit](https://github.com/slowmist/Knowledge-Base/blob/master/open-report/Smart%20Contract%20Security%20Audit%20Report%20-%20PlexSwap%20Lottery.pdf)
* Transparent:
  * We’re built on open-source software: our site and all our Smart Contracts are publicly visible for maximum transparency.
  * Our contracts are verified on BscScan so you know that what you see is what you get: [1](https://bscscan.com/address/0x10ED43C718714eb63d5aA57B78B54704E256024E) [2](https://bscscan.com/address/0x73feaa1ee314f8c655e354234017be2193c9e24e#code) [3](https://bscscan.com/address/0xbcfccbde45ce874adcb698cc183debcf17952812) [4](https://bscscan.com/address/0x1b96b92314c44b159149f7e0303511fb2fc4774f#code) [5](https://bscscan.com/address/0x92E8CeB7eAeD69fB6E4d9dA43F605D2610214E68)
* Security best practices:
  * The chefs use multisig for all contracts.
  * Our contracts’ time-lock gives you peace of mind.

## How can I stake WAYA?

You can stake your WAYA in PlexSwap Gaya Pools. Visit the [Gaya Pools page](https://PlexSwap.finance/pools).

Read our [How to Stake in Gaya Pools guide](https://docs.PlexSwap.finance/products/gaya-pool/gaya-pool-guide) if you'd like a hand getting started with staking.

## What is the difference between staking and farming?

Staking in Gaya Pools and farming with Yield Farming are both ways to earn more WAYA by supporting PlexSwap.

Staking only needs some WAYA to be added to a Gaya Pool to earn WAYA or other tokens.\
[Learn more about Gaya Pool staking.](https://docs.PlexSwap.finance/products/gaya-pool)

Farming is more complicated and needs LP Tokens to earn WAYA.\
[Learn more about Yield Farming.](https://docs.PlexSwap.finance/products/yield-farming)

## How do I farm?

We have a [Yield Farming guide](https://docs.PlexSwap.finance/products/yield-farming/how-to-use-farms) if you're interested in learning how to farm.

## Where can I view the PlexSwap roadmap?

You can [view our to-do list here, but don't call it a roadmap](https://docs.PlexSwap.finance/roadmap).

## How do I connect my wallet to BNB Smart Chain and PlexSwap?

We have a [Connect Your Wallet to PlexSwap guide](https://docs.PlexSwap.finance/get-started/connection-guide) covering this in detail.

## What's the best wallet for PlexSwap?

It depends on your needs. We have an [in-depth guide to selecting and creating a wallet](https://docs.PlexSwap.finance/get-started/wallet-guide) that's right for you.

## Why is my transaction failing?

You can check the status of a transaction on [https://bscscan.com/](https://bscscan.com).

Our [Troubleshooting Errors guide](https://docs.PlexSwap.finance/help/troubleshooting) may have a solution for your problem if you're having issues.

You can also see our [Fixing Stuck Pending Transactions guide](https://docs.PlexSwap.finance/help/unsticking-a-transaction-stuck-as-pending-with-metamask) if you have a stuck transaction.

## When will you open more pools?

New Pools are added to PlexSwap frequently. There will always be an announcement before the launch of new pools.

Join the [announcements Telegram group](https://t.me/PlexSwapAnn) to learn about new Pools as early as possible.

## Did Farm APR calculation change?

Previously, rewards earned by LP Token-holders generated from trading fees were not included in Farm APR calculations. APR calculations now include these rewards, and better reflect the expected APR for Farm pairs.

## How do I get airdrops?

Whenever there is an official airdrop on PlexSwap it will be announced along with the requirements.

Please remember anyone can airdrop tokens to PlexSwap users since every transaction is public on BscScan. Be sure to do your own research when it comes to non-official airdrops. To protect your funds, we recommend you don't use a smart contract you don't understand from a source you don't trust.

## How can I report a bug?

Learn about our [bug bounty and potential bounty payouts](https://docs.PlexSwap.finance/code/bug-bounty).

## Where can I view smart contracts?

Learn how to find smart contracts on our [Finding Contracts page](https://docs.PlexSwap.finance/code/smart-contracts).

## Why does it say I have no BNB balance?

If you've already [transferred BNB into your BNB Smart Chain-enabled wallet](https://docs.PlexSwap.finance/get-started/bep20-guide) but still have this error, you're most likely not [connected to BNB Smart Chain](https://docs.PlexSwap.finance/get-started/connection-guide) within your wallet. Check your wallet's selected network and make sure you have BNB Smart Chain (BSC) selected.

## How do I vote?

To learn more about voting, you can [read our section on Voting](https://docs.PlexSwap.finance/products/voting), including voting guides.

## What is the max supply of WAYA?

$WAYA does not have a maximum supply. The circulating supply is managed through built-in burning and regular burning events.\
\
Read this to [learn more about PlexSwap's tokenomics](https://docs.PlexSwap.finance/tokenomics/waya).

## What are the treasury funds used for?

The treasury funds are used to cover the expenses involved in running PlexSwap. These expenses include salaries, audits, prizes, hosting, upkeep, bounties, etc.

## Where can I check the Analytics?

You can check the analytics of PlexSwap by click on the "Analytics" tab on the top menu or by clicking the link below.

Analytics: [https://PlexSwap.info/](https://PlexSwap.info)

## Is PlexSwap protected from flashloan attacks?

PlexSwap's vault has anti-flashloan protection. PlexSwap’s WAYA token isn’t vulnerable to flash loan attacks. Unlike vulnerable tokens, WAYA token minting is predefined, and can’t be adjusted in a single transaction. Ownership cannot be transferred outside of MasterChef contract.

PlexSwap’s other smart contracts, like IFO and AutoPool, are protected as well; they prevent other contracts from interacting with them, reducing the scope of vector attacks.

## Can I join the PlexSwap team?

Check the [Become a Chef](https://docs.PlexSwap.finance/hiring/become-a-chef) area for information on open positions we're looking to fill.

We advertise new positions we're looking to fill on our [official social media channels](https://docs.PlexSwap.finance/contact-us/telegram), so be sure to follow us to get the latest hiring information.

## What is GAYA?

GAYA was a part of the staking process earlier in PlexSwap's life. GAYA was discontinued when a security issue was discovered and is no longer a part of PlexSwap.

## I can't find an answer for my question. Where do I find an answer?

If you can't find what you're looking for in PlexSwap's documentation, ask your question on [PlexSwap's official social media platforms](https://docs.PlexSwap.finance/contact-us/telegram) and someone will do their best to help you out.

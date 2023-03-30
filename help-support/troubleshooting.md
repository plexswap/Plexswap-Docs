# Troubleshooting Errors

Sometimes you may find yourself facing a problem that doesn't have a clear solution. These troubleshooting tips may help you solve problems you run into.

## **Issues on the Exchange**

### **INSUFFICIENT\_OUTPUT\_AMOUNT**

> The transaction cannot succeed due to error: PlexswapRouter: INSUFFICIENT\_OUTPUT\_AMOUNT. This is probably an issue with one of the tokens you are swapping.
>
> the transaction cannot succeed due to error: execution reverted: plexswaprouter: insufficient\_output\_amount.

You're trying to swap tokens, but your slippage tolerance is too low or liquidity is too low.

{% tabs %}
{% tab title="Solution" %}
1. Refresh your page and try again later.
2. Try trading a smaller amount at one time.
3. Increase your slippage tolerance:
   1. Tap the settings icon on the liquidity page.
   2. Increase your slippage tolerance a little and try again. ![](<../.gitbook/assets/liquidity\_settings (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)
4. Lastly, try inputting an amount with fewer decimal places.
{% endtab %}

{% tab title="Reason" %}
**This usually happens when trading tokens with low liquidity.**

That means there isn't enough of one of the tokens you're trying to swap in the Liquidity Pool: it's probably a small-cap token that few people are trading.

However, there's also the chance that you're trying to trade a scam token which cannot be sold. In this case, PlexSwap isn't able to block a token or return funds.
{% endtab %}
{% endtabs %}

### **INSUFFICIENT\_A\_AMOUNT or INSUFFICIENT\_B\_AMOUNT**

> Fail with error 'PlexswapRouter: INSUFFICIENT\_A\_AMOUNT'\
> or\
> Fail with error 'PlexswapRouter: INSUFFICIENT\_B\_AMOUNT'

You're trying to add/remove liquidity from a liquidity pool (LP), but there isn't enough of one of the two tokens in the pair.

{% tabs %}
{% tab title="Solution" %}
**Refresh your page and try again, or try again later.**

Still doesn't work?

1. Tap the settings icon on the liquidity page.
2. Increase your slippage tolerance a little and try again.

![](<../.gitbook/assets/liquidity\_settings (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)
{% endtab %}

{% tab title="Reason" %}
The error is caused by trying to add or remove liquidity for a liquidity pool (LP) with an insufficient amount of token A or token B (one of the tokens in the pair).

It might be the case that prices are updating too fast when and your slippage tolerance is too low.
{% endtab %}
{% endtabs %}

### PlexswapRouter: EXPIRED

> The transaction cannot succeed due to error: PlexswapRouter: EXPIRED. This is probably an issue with one of the tokens you are swapping.

Try again, but confirm (sign and broadcast) the transaction as soon as you generate it.

This happened because you started making a transaction, but you didn't sign and broadcast it until it was past the deadline. That means you didn't hit "Confirm" quickly enough.

### Plexswap: TRANSFER\_FAILED

> The transaction cannot succeed due to error: execution reverted: Plexswap: TRANSFER\_FAILED.

Make sure you have 30% more tokens in your wallet than you intend to trade, or try to trade a lower amount. If you want to sell the maximum possible, try 70% or 69% instead of 100%.\
Caused by the design of Restorative Rebase tokens like tDoge or tBTC.\
[Understand how restorative rebase tokens work](https://btcst.medium.com/stp-8-restorative-rebase-b4fbbdfd96c).

Another possible cause of this issue is the malicious token issuer just suspended the trading for their token. Or they made selling action only possible for selected wallet addresses. Please always do your own research to avoid any potential fraud. If the token you are trying to swap but failed with this error code is coming from an airdrop, that is most likely a scam. Please do not perform any token approval or follow any links, your fund may be at risk if you try to do so.

### Transaction cannot succeed

Try trading a smaller amount, or increase slippage tolerance via the settings icon and try again. This is caused by low liquidity.

### **Price Impact too High**

Try trading a smaller amount, or increase slippage tolerance via the settings icon and try again. This is caused by low liquidity.

### Cannot read property 'toHexString' of undefined

> "Unknown error: "Cannot read property 'toHexString' of undefined"

When trying to swap tokens, the transaction fails and this error message is displayed. This error has been reported on mobile devices using Trust Wallet.

{% tabs %}
{% tab title="Solution" %}
1. Attempt the transaction again with increased slippage allowance.
2. If 1. does not resolve your problem, consider using another wallet such as SafePal for your transaction.
{% endtab %}

{% tab title="Reason" %}
**This usually happens when trading tokens with insufficient slippage allowance on Trust Wallet.**

The exact details of the problem are still being investigated.
{% endtab %}
{% endtabs %}

### **Execution reverted: TransferHelper: TRANSFER\_FROM\_FAILED.**

> The transaction cannot succeed due to error: execution reverted: TransferHelper: TRANSFER\_FROM\_FAILED.

When trying to swap tokens, the transaction fails and this error message is displayed. This error has been reported across platforms.

{% tabs %}
{% tab title="Solution" %}
1. Check to make sure you have sufficient funds available.
2. Ensure you have given the contract allowance to spend the amount of funds you're attempting to trade with.
{% endtab %}

{% tab title="Reason" %}
This error happens when trading tokens with insufficient allowance, or when a wallet has insufficient funds.\
If you're trading tokens with Restorative Rebase like tau assets tDoge or tBTC, make sure you understand how they work first with this [guide to Rebase tokens](https://btcst.medium.com/stp-8-restorative-rebase-b4fbbdfd96c).
{% endtab %}
{% endtabs %}

## **Issues with Crop Silos**

### Out of Gas error

> Warning! Error encountered during contract execution \[out of gas]

You have set a low gas limit when trying to make a transaction.

{% tabs %}
{% tab title="Solution" %}
Try manually increasing the **gas limit** (not gas price!) in your wallet before signing the transaction.

A limit of 200000 is usually enough.

![](<../.gitbook/assets/image (2).png>)

The above example is from Metamask; check your wallet's documentation if you aren't sure how to adjust the gas limit.
{% endtab %}

{% tab title="Reason" %}
Basically, your wallet (Metamask, Trust Wallet, etc.) can't finish what it's trying to do.

Your wallet estimates that the gas limit is too low, so the function call runs out of gas before the function call is finished.
{% endtab %}
{% endtabs %}

### BEP20: transfer amount exceeds allowance

> Fail with error 'BEP20: transfer amount exceeds allowance'

{% tabs %}
{% tab title="Solution" %}
1. Use Unrekt.net to revoke approval for the smart contract you're trying to interact with
2. Approve the contract again, without setting a limit on spend allowance
3. Try interacting with the contract again.
{% endtab %}

{% tab title="Reason" %}
This happens when you set a limit on your spend allowance when you first approved the contract, then try to swap more than the limit.
{% endtab %}
{% endtabs %}

### BEP20: transfer amount exceeds balance

> Fail with error 'BEP20: transfer amount exceeds balance'

You're probably trying to unstake from a Crop Silo with low rewards in it. Solution below.

If not, you may be trying to send tokens that you don't have in your wallet (for example, trying to send a token that is already assigned to a pending transaction). In this case, just make sure you have the tokens you're trying to use.

{% tabs %}
{% tab title="Solution" %}
Firstly,[ let the team know](broken-reference/) which pool you're trying to unstake from, so they can top up the rewards. If you're in a hurry to unstake and you don't mind losing your pending yield, try an emergencyWithdraw:

You can perform an “emergencyWithdraw” from the contract directly to unstake your staked tokens.

1. Find the contract address of the Crop Silo you're trying to unstake from. You can find it in your wallet's transaction log.
2. Go to [https://bscscan.com/](https://bscscan.com/address/0x73feaa1eE314F8c655E354234017bE2193C9E24E#writeContract) and in the search bar, enter the contract address.
3. Select **Write Contract.**
4. Click **“Connect to Web3”** and connect your wallet.![](https://lh6.googleusercontent.com/-\_sNkO1gcOOJXkduDEUzbExKE2mNxBOR0f86Lpp3BBuPbIcmAHsfuvpF-hKqRn4oID5QzdGkk\_1dTHkPuCmE50vpNNZxEqoM5nPmE\_12k3-8Q8YYoRYqJ\_VGjxJ03YPRuVQ1O5ME)
5. In section **“3. emergencyWithdraw”,** and click “Write”.

This will unstake your staked tokens and lose any uncollected yield.

{% hint style="warning" %}
**This will lose any yield that you haven’t harvested yet.**
{% endhint %}
{% endtab %}

{% tab title="Reason" %}
This error tends to appear when you're trying to unstake from an old Crop Silo, but there aren't enough rewards in the pool left for you to harvest when withdrawing. This causes the transaction to fail.
{% endtab %}
{% endtabs %}

## **Other issues**

### Provider Error

> Provider Error\
> No provider was found

This happens when you try to connect via a browser extension like MetaMask or Binance Chain Wallet, but you haven’t installed the extension.

{% tabs %}
{% tab title="Solution" %}
Install the official browser extension to connect, or read our guide on [how to connect a wallet to PlexSwap](https://docs.plexfinance.us/plexswap/get-started/connection-guide).
{% endtab %}
{% endtabs %}

### Unsupported Chain ID

Switch your chain to BNB Smart Chain. Check your wallet's documentation for a guide if you need help.

### Already processing eth\_requestAccounts. Please wait.

Make sure you are signed in to your wallet app and it's connected to BNB Smart Chain.

### Issues buying PLEX-F and similar tokens

To trade PLEX-F, you must click on the settings icon and **set your slippage tolerance to 12% or more.**\
This is because **PLEX-F taxes approximately a 10% fee on each transaction**:

* 4.5% fee = redistributed to all existing holders
* 3% fee = used to add liquidity
* 2% fee = used to finance project development
* 0.5% fee = used to compose a contingency fund

This is also why you might not receive as much of the token as you expect when you purchase.\
Read more on [PLEX-F Fundamentals](https://finance.symplexia.com/fundamentals/).

### Internal JSON-RPC errors

> "MetaMask - RPC Error: Internal JSON-RPC error. estimateGas failed removeLiquidityETHWithPermitSupportingFeeOnTransferTokens estimateGas failed removeLiquidityETHWithPermit "

Happens when trying to remove liquidity on some tokens via Metamask. Root cause is still unknown. Try using an alternative wallet.

> Internal JSON-RPC error. { "code": -32000, "message": "insufficient funds for transfer" } - Please try again.

You don't have enough BNB to pay for the transaction fees. You need more BEP-20 network BNB in your wallet.

### Error: \[ethjs-query]

> Error: \[ethjs-query] while formatting outputs from RPC '{"value":{"code":-32603,"data":{"code":-32000,"message":"transaction underpriced"\}}}"

Increase the gas limit for the transaction in your wallet. Check your wallet's documentation to learn how to increase gas limit.

> Swap failed: Error: \[ethjs-query] while formatting outputs from RPC '{"value":{"code":-32603,"data":{"code":-32603,"message":"handle request error"\}}}'

Cause unclear. Try these steps before trying again:

1. Increase gas limit
2. Increase slippage
3. Clear cache

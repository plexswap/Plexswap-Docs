# BOOSTERS

![](../.gitbook/assets/Get\_Started.png)

 Farm Boosters, is an automatic generated boost multiplier that allows you to boost your WAYA yield from selected farms up to 2x, taking full advantage of combining fixed-term WAYA staking and liquidity yield farming.

**A Booster is NOT a new kind of token and can NOT be transferred!**


## How are the multipliers calculated?

In order to provide an attractive boost for liquidity farming while serving as an incentive for WAYA staking, bWAYA multipliers are calculated based on various metrics from the WAYA staking pool and the farm you choose to boost.

### The most important metrics

Farm Boosters multipliers are calculated using the following metrics upon activation or refresh:

*   The number of WAYA you stake in the fixed-term staking position (userLockedAmount)
*   The duration of your fixed-term staking position (userLockedDuration)
*   The number of LP tokens you stake in the farm (userLpStakedAmount)

Meanwhile, to ensure the system is fair and beneficial to the entire Plexswap ecosystem. The calculation will also take into account the overall staking performance of the WAYA pool and farms. Therefore, the following global metrics are also included in the calculation:

*   The total amount of WAYA locked in the fixed-term WAYA staking pool (totalLockedAmount)
*   The average lock duration of the fixed-term WAYA staking pool (averageLockedDuration)
*   The total amount of LP tokens staked in the farm (totalLpStakedAmount)

The final multipliers will reflect each user’s performance against the entire WAYA pool and farm. Therefore, when you try to boost different Plexswap farms, you may get a different boost multiplier.

### Calculation formulas

The multiplier is calculated using the following formulas:

1. resultA = constantA * userLpStakedAmount
2. resultB = (totalLpStakedAmount * userLockedAmount * userLockedDuration / constantB) / (totalLockedAmount * averageLockedDuration)
3. boostMultiplier = min(userLpStakedAmount, (resultA + resultB)) / resultA

constantA and constantB are set by the kitchen and subject to future adjustments based on community feedback and market condition.

### Multiplier auto refresh

It is important to note that any user actions to the farms or WAYA staking pool will automatically update your boost multiplier based on the latest data and statistics from farms and the WAYA staking pool, including but not limited to:

*   Stake/Unstake LP tokens to/from Farm
*   Harvest WAYA rewards from Farm
*   Extend your WAYA staking duration
*   Add more WAYA into your fixed-term staking position
*   Convert your WAYA staking position to flexible
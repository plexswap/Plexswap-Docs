#Waya Silo FAQ

## FAQ

### What lock duration can we choose?

You can choose from 1-52 weeks. What do you prefer?

### What variables affect the Waya Silo APYs (Flexible and Fixed-Term Staking options)?

Since flexible staking and fixed-term staking options are part of the same pool, the following variables affect the APY of both:

* Total WAYA staked in flexible staking and fixed-term staking (the sum of both). The more WAYA staked, the lower the APY.
* Total locked WAYA in fixed-term staking. The more WAYA locked means more yield boosts, resulting in fewer WAYA rewards for others (especially flexible staking).
* The average lock duration of all WAYA locked in fixed-term staking. If the average lock duration increases, APY will decrease.

### Can I harvest the rewards during the locked period?

No. You can harvest the rewards only when the locked duration is ended. This is based on the yield/return we are providing as well as the technical implementations.

### Can I extend the lock duration?

Yes. Extending the lock duration adds more time to your **initial lock duration**. When choosing to extend your lock duration, note:

New extended lock duration = initial lock duration + added duration

### Can I remove my WAYA from Fixed-Term staking via contract if I change my mind?

No. Your WAYA cannot be removed or withdrawn from fixed-term staking at any point in time until your lock duration ends and your WAYA is unlocked.

### What is the "WAYA Locked" amount?

The "WAYA Locked" amount is a user's initial locked WAYA balance plus WAYA rewards to date.&#x20;

WAYA Locked = Initial locked WAYA balance + WAYA rewards

When adding more WAYA to fixed-term staking, the "WAYA to be locked" amount is the user's initial locked WAYA balance, WAYA rewards to date, and the WAYA being added.

### Can the Fixed-Term Staking WAYA Silo APY change after I lock my WAYA?

Yes, the fixed-term staking WAYA Silo APY is variable, just like the old WAYA Silos. The fixed-term staking WAYA Silo APY is not fixed and is dependent on:

* Total WAYA staked in the WAYA Silo (the sum of both Flexible + Fixed-Term Staking).
* The average lock duration of all WAYA locked in fixed-term staking.
* A yield boost (similar to a multiplier) calculated from a user's initial lock duration. The longer you lock your WAYA, the higher the yield boost.

For example, if you lock your WAYA for 52 weeks, your yield boost will be larger than if you lock your WAYA for 26 weeks. The yield boost increases linearly the longer you lock your WAYA.

### Can I still participate in IFOs if my WAYA is locked in the Fixed-Term Staking pool, or will I need to buy more WAYA?

TBD, more information will be provided soon.

### Can I vote if my WAYA is locked in the Fixed-Term Staking pool?

TBD, more information will be provided soon.

### Can I use both the Flexible Staking WAYA Silo and the Fixed-Term Staking WAYA Silo at the same time?

No. As mentioned above in the "What’s the difference" section, both options are part of the same, single pool. You currently can **never** have WAYA in both fixed-term and flexible staking.

We have multiple solutions coming in the future to allow users to use both flexible staking and fixed-term staking at the same time, but for now, you can choose only one of them.

### Is there a fee for converting Flexible Staked WAYA to Fixed-Term Staked WAYA?

No. There are no additional fees for moving WAYA from flexible staking to fixed-term staking, only network fees.

### What happens at the end of the lock duration? What is "After Burning"?

When your fixed-term staking period ends, and your WAYA unlocks, you have 7 days to complete one of two options:

* Lock your WAYA to begin a new fixed-term staking period\
  or
* Convert your staked WAYA to flexible staking (no 72-hour withdrawal fee).

![](../../../.gitbook/assets/waya-silo-lock-end.png)

During these 7 days, you will still earn WAYA at the same APY as your lock period.

After 7 days, if you have not done one of the two options, your staked WAYA will enter what is called "After Burning". In "After Burning", you will still earn WAYA, but a portion of your rewards will be sent to burn at a linearly decreasing APR over 90 days, where your APR will be 0% after 90 days.

The “After Burning” state will last for 90 days until all the WAYA rewards are burnt. So, to avoid missing out on WAYA rewards, we recommend starting a new fixed-term staking period or converting your WAYA to flexible staking at the end of your lock staking period.

![](<../../../.gitbook/assets/waya-silo-lock-burn (1).png>)

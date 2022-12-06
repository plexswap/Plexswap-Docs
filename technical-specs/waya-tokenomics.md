# WAYA Tokenomics

![](../../.gitbook/assets/220628-en.png)

## **Emission rate** <a href="#emission-rate" id="emission-rate"></a>

### **Per block**

| **Metric**             | **Emission/block (WAYA)** | **Emission/day (WAYA)** |
| ---------------------- | ------------------------: | ----------------------: |
| Emission               |                        40 |               1,152,000 |
| Burned Weekly          |                    -26.25 |                -756,000 |
| **Effective Emission** |              **<13.75\*** |           **350,000\*** |

\*Effective Emission might be in fact slightly below this amount.

In addition to the above, a dynamic amount of WAYA is also [minted to the Dev address](https://bscscan.com/address/0xceba60280fb0ecd9a5a26a1552b90944770a4a0e#tokentxns) at a rate of 9.09%. This means that if 100 WAYA are harvested, then 9.09 WAYA is minted in addition and sent to the Dev Address.

{% hint style="info" %}
All WAYA minted to the Dev address is burned in the weekly burn and never enters circulation.&#x20;

As such, we haven't included it in the above emission rate.
{% endhint %}

## Distribution <a href="#distribution" id="distribution"></a>

| Distributed to                | Reward/block (% of emission) | Reward/block (total WAYA) |           Reward/day |
| ----------------------------- | ---------------------------: | ------------------------: | -------------------: |
| Farms              |                        9.37% |                      3.75 |     108,000 (approx) |
| of which diverted and burned  |                              |                           |              -46,000 |
| Crop Silos                   |                          25% |                        10 |     288,000 (approx) |
| **Total Daily WAYA Emission** |                              |                           | **350,000 (approx)** |

## **Other Deflationary Mechanics** <a href="#other-deflationary-mechanics" id="other-deflationary-mechanics"></a>

{% hint style="info" %}
The burning process is currently manual. [View burn transactions here](https://bscscan.com/token/0x32d9F70F6eF86718A51021ad269522Abf4CFFE49?a=0x000000000000000000000000000000000000dead).
{% endhint %}

As well as the above, WAYA is also burned in the following ways:

* **0.0575%** of every trade made on PlexSwap 
* **100%** of WAYA sent to the Dev address
* **2%** of every yield harvest from all the flexible staking positions in WAYA Silo

## Why is the WAYA burn manual?

To hit the ground running, PlexSwap launched as an MVP (minimum viable product) with the ChiefMaster contract emitting 40 WAYA per block. For that reason, the early team didn't add additional functions such as the ability to customize the WAYA minting logic. The team has been controlling WAYA emissions through a manual burn process by creating the following pool:

* Burn Pool (PID - 138) - burned WAYA per block

These pools work similarly to the farms, where the Farmers can adjust the percentage of the 40 WAYA per block allocated to it after each WAYA emission reduction vote.

The ratio of the WAYA burn per block is controlled by the ChiefFarmer contract. This allows the burn to be much more accurate.

{% hint style="warning" %}
On the day of the burn, the supply shown on the homepage might suddenly jump by several million WAYA.&#x20;

Don't worry - **THIS WAYA NEVER ACTUALLY ENTERS CIRCULATION:**
{% endhint %}

This apparent jump is just because of how all the WAYA that's allocated for the burn is stored during the week.&#x20;

The WAYA allocated to burn are harvested before completing the weekly token burns, and this makes the Total Supply shown on the site jump by \~6M. This is because pending WAYA sometimes doesn't get registered in the Total Supply until it's harvested on the burn day. Once the token burn transaction is completed, the \~6M is shown in the Burned to Date.&#x20;

## How to Confirm WAYA Supply for yourself

To confirm that the circulating WAYA supply shown on the PlexSwap homepage is correct,&#x20;

1. Head to the WAYA token contract on BscScan and [see how much WAYA is held by the Burn Address.](https://bscscan.com/token/0x32d9F70F6eF86718A51021ad269522Abf4CFFE49#balances) That's the total amount of WAYA that's been burned (removed from circulation FOREVER, and impossible to ever retrieve).
2. Then, subtract this burned amount from the "Total Supply" that BscScan shows.
3. This gives you the actual WAYA supply.



#### **Read more about WAYA's deflationary mechanics on the next page.** <a href="#read-more-about-wayas-deflationary-mechanics-on-the-next-page" id="read-more-about-wayas-deflationary-mechanics-on-the-next-page"></a>

# Non-Market Capitalization Weighted Indices

## Non-Market Capitalization Weighted Indices

A non-market capitalization weighted index (also referred to as a non-market cap or modified market cap index) is one where the weights of the index constituents are not determined by the market capitalization weighted methodology. For example, the weights are user-defined. Between index rebalancing, most corporate actions generally don't affect index weights, as they are fixed. As the constituents' price move, their weights will change accordingly. Therefore, a non-market capitalization weighted index must be rebalanced from time to time to reestablish proper weighting.

The overall approach to calculating non-market capitalization weighted indices is the same as the capitalization weighted indices. However, the constituents' market value are set to a value to achieve a specific weight at each rebalancing that is different from a purely circulating-adjusted market capitalization weighting.

The index level of a non-market capitalization weighted index is calculated by:

$$
{Index Level}=\frac{{Index Value}}{{Divisor}}
$$

The _IndexValue_ is calculated by:

$$
{Index Value}={\sum_{i} P_{i} * Q_{i}}
$$

Where the _IndexValue_ is the market value of an index with all constituents' circulating market capitalization; _Pi_ is the price of each constituent in the index, _Qi_ is the quantity of each constituent's circulating supply, and _i_ denotes a constituent.

However, to calculate a non-market capitalization weighted index, the market value for each constituent in the index is redefined so that it has the appropriate weight in the index at the initial calculation date and also at each rebalancing date. The new adjustment factor used to establish the appropriate weighting is called Weight Adjustment Factor (WAF).&#x20;

Therefore, the constituent market value is calculated by:

$$
\text {CV}_{i}={P_{i} * Q_{i} * WAF_{i}}
$$

Where _CVi_ is the market value of constituent _i_, _Pi_ is the price of constituent _i_, _Qi_ is the quantity of the circulating supply of constituent _i,_ and W_AFi_ is the adjustment factor of constituent _i_.

Therefore, the index level is calculated by:

$$
{Index Level}=\frac{\sum_{i} CV_{i}}{{Divisor}}
$$

And, the WAF for each index constituent _i_ on rebalancing date _t_ is calculated by:

$$
{WAF}_{i,t}=\frac{{AW}_{i,t}}{{W}_{i,t}}
$$

Where A_Wi,t_ is the assigned weight of constituent _i_ on rebalancing date _t_ as determined by the weighting rule of the index in question, and _Wi,t_ is the original weight of constituent _i_ on rebalancing date _t_ based on the circulating-adjusted market capitalization.

The index divisor is defined based on the index level and market value. The index level stays unchanged at the rebalancing. But the divisor will change at the rebalancing, since prices and circulating supplies will have changed since the last rebalancing.

Therefore, the divisor is calculated by:

$$
{{Divisor}}_{after}=\frac{{Index Value}_{after}}{{Index Value}_{before}}
$$

### An example

Let's assume we are constructing a non-market capitalization weighted index named XYZ, composed of three constituents X, Y, and Z with the user-assigned weights of 25%, 35% and 40% for X, Y, and Z, respectively. The price and quantity of circulating supply for each constituent are shown in the table:&#x20;

| Constituent | Price (USD) | Quantity (USD) |
| ----------- | ----------- | -------------- |
| X           | 100         | 2,000,000      |
| Y           | 200         | 5,000,000      |
| Z           | 300         | 8,000,000      |

The original weight of each constituent before adjustment is shown below:

| Constituent | Original Weight |
| ----------- | --------------- |
| X           | 5.555%          |
| Y           | 27.778%         |
| Z           | 66.667%         |

The weights after adjustments are:

| Constituent | Adjusted Weight | WAF  |
| ----------- | --------------- | ---- |
| X           | 25%             | 4.50 |
| Y           | 35%             | 1.26 |
| Z           | 40%             | 0.60 |

We set the divisor to 36,000,000 USD. Therefore, the index level of XYZ is:

$$
{XYZ}=\frac{(100*2000000*4.50)+(200*5000000*1.26)+(300*8000000*0.60)}{36000000} = 100
$$

## Equal Weighted Indices

An equal weighted index is one where the index constituents have the same weight. As the constituents' price change, their weights will shift and break the exact equality. Therefore, an equal weighted index must be rebalanced from time to time to reestablish the equal weighting.

The overall approach to calculating equal weighted indices is the same as the capitalization weighted indices. However, the constituents' market value are set to a value to achieve a specific weight at each rebalancing that is different from a purely circulating-adjusted market capitalization weighting.

The index level of an equal weighted index is calculated by:

$$
{Index Level}=\frac{{Index Value}}{{Divisor}}
$$

The _IndexValue_ is calculated by:

$$
{Index Value}={\sum_{i} P_{i} * Q_{i}}
$$

Where the _IndexValue_ is the market value of an index with all constituents' circulating market capitalization; _Pi_ is the price of each constituent in the index, _Qi_ is the quantity of each constituent's circulating supply, and _i_ denotes a constituent.

However, to calculate an equal weighted index, the market value for each constituent in the index is redefined so that it has the same weight in the index at the initial calculation date and also at each rebalancing date. The new adjustment factor used to establish the appropriate weighting is called Equal-Weighted Adjustment Factor (EWAF).&#x20;

Therefore, the constituent market value is calculated by:


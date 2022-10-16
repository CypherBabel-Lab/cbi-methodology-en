# Market Capitalization Weighted Indices

A majority of CBI’s crypto asset indices are market capitalization weighted and circulating-adjusted, where each crypto asset’s weight in the index is proportional to the total market value of its circulating supply. This is analogous to the free-float capitalization in the stock market.

CBI also provides capped versions of a market capitalization weighted index where single index constituents or defined groups of index constituents, such as sector or group, are confined to a maximum weight.

## Market Capitalization Weighted Index

Most of the CBI indices are market capitalization weighted indices. Sometimes these are called value weighted or market cap weighted. A constituent's weight of a market capitalization weighted index is proportional to its market capitalization determined by its circulating supply.&#x20;

The index level of a market capitalization weighted index is calculated by:

$$
{Index Level}=\frac{{Index Value}}{{Divisor}}
$$

Where the numerator on the right-hand side is the market value of an index with all constituents' circulating market capitalizations. This is summed across all the constituents in the index. The denominator is the divisor. If the numerator is US$ 1.0 trillion and the divisor is US$ 10 billion, the index level would be 100.

The _IndexValue_ is calculated by:

$$
{Index Value}={\sum_{i} P_{i} * Q_{i}}
$$

Where _Pi_ is the price of each constituent in the index, _Qi_ is the quantity of each constituent's circulating supply, and _i_ denotes a constituent.

The weight of a constituent is calculated by:

$$
{W}_{i}=\frac{{P}_{i}*{Q}_{i}}{{Index Value }}
$$

Where _Pi_ is the price of constituent _i_, _Qi_ is the quantity of the circulating supply of constituent _i,_ and _IndexValue_ is the market value of an index with all constituents' circulating market capitalizations.

{% hint style="info" %}
The real-time price and quantity data for the constituents in CBI indices are provided by well-established data aggregators, including CoinGecko and CoinMarketCap.&#x20;
{% endhint %}

### An example

Let's assume we are constructing a market capitalization weighted index named XYZ, which is composed of three constituents X, Y, and Z. The price and quantity of circulating supply for each constituent are shown in the table:&#x20;

| Constituent | Price (US Dollar) | Quantity  |
| ----------- | ----------------- | --------- |
| X           | 100               | 2,000,000 |
| Y           | 200               | 5,000,000 |
| Z           | 300               | 8,000,000 |

We set the divisor to 36,000,000 USD. Therefore the index level of XYZ is:

$$
{XYZIndexLevel}=\frac{(100*2000000)+(200*5000000)+(300*8000000)}{36000000} = 100
$$

And the weight of each constituent is:

| Constituent | Weight  |
| ----------- | ------- |
| X           | 5.555%  |
| Y           | 27.778% |
| Z           | 66.667% |

## Capped Market Capitalization Weighted Index

A capped market capitalization weighted index is one where single index constituents or defined groups of index constituents are confined to maximum weight. The excess weight is distributed proportionately among the remaining index constituents. Sometimes, it is also called a capped market cap index, capped index or capped weighted index. As constituent prices change the weights will shift, and the modified weights will change. Therefore, a capped market cap weighted index must be rebalanced from time to time to re-establish proper weighting.&#x20;

The calculation for capped indices is identical to market capitalization weighted indices, except that the indices use an additional weight factor to adjust the market capitalization to a value such that the index weight constraints are satisfied. For capped indices, no change is made on the additional weight factor due to project or corporate actions between rebalancing calculations. Therefore, the weights of constituents in the index will change due to market capitalization changes.&#x20;

The index level is calculated by:

$$
{Index Level}=\frac{{Index Value}}{{Divisor}}
$$

Where the numerator on the right-hand side is the market value of an index with all constituents' circulating market capitalizations. This is summed across all the constituents in the index. The denominator is the divisor.&#x20;

The _IndexValue_ is calculated by:

$$
{Index Value}={\sum_{i} P_{i} * Q_{i}}
$$

Where _Pi_ is the price of each constituent in the index, _Qi_ is the quantity of each constituent's circulating supply, and _i_ denotes a constituent.

However, to calculate a capped index, the market capitalization for each constituent in the index is redefined so that it has the appropriate weight in the index at the initial calculation date and also each rebalancing date. The new adjustment factor used to establish the appropriate weighting is called Capped Market Capitalization Adjustment Factor (CMCAF).&#x20;

Therefore, the constituent market value is calculated by:

$$
\text {CV}_{i}={P_{i} * Q_{i} * CMCAF_{i}}
$$

Where _CVi_ is the market value of constituent _i_, _Pi_ is the price of constituent _i_, _Qi_ is the quantity of the circulating supply of constituent _i,_ and _CMCAFi_ is the adjustment factor of constituent _i_.

Therefore, the index level is calculated by:

$$
{Index Level}=\frac{\sum_{i} CV_{i}}{{Divisor}}
$$

And, the CMCAF for each index constituent _i_ on rebalancing date _t_ is calculated by:

$$
{CMCAF}_{i,t}=\frac{{CW}_{i,t}}{{W}_{i,t}}
$$

where _CWi,t_ is the capped weight of constituent _i_ on rebalancing date _t_ as determined by the capping rule of the index in question, and _Wi,t_ is the uncapped weight of constituent _i_ on rebalancing date _t_ based on the circulating-adjusted market capitalization of all index constituents.

The index divisor is defined based on the index level and market value. The index level stays unchanged at the rebalancing. But the divisor will change at the rebalancing since prices and circulating supplies will have changed since the last rebalancing.

Therefore, the divisor is calculated by:

$$
{{Divisor}}_{after}=\frac{{Index Value}_{after}}{{Index Value}_{before}}
$$

Where:

$$
{Index Value}_{after}={\sum_{i} P_{i} * Q_{i}} * {CMCAF}_{i}
$$

### An example

Let's assume we are constructing a capped market capitalization weighted index named XYZ, composed of three constituents X, Y, and Z. The cap for index XYZ is set to 50%.  The price and quantity of circulating supply for each constituent are shown in the table:&#x20;

| Constituent | Price (USD) | Quantity (USD) |
| ----------- | ----------- | -------------- |
| X           | 100         | 2,000,000      |
| Y           | 200         | 5,000,000      |
| Z           | 300         | 8,000,000      |

The uncapped weight of each constituent before adjustment is shown below:

| Constituent | Uncapped Weight |
| ----------- | --------------- |
| X           | 5.555%          |
| Y           | 27.778%         |
| Z           | 66.667%         |

The uncapped weight of constituent Z does not satisfy the cap of the index. Hence, the weights of constituents are adjusted accordingly:

| Constituent | Capped Weight | CMCAF |
| ----------- | ------------- | ----- |
| X           | 8.333%        | 1.50  |
| Y           | 41.667%       | 1.50  |
| Z           | 50.000%       | 0.75  |

We set the divisor to 36,000,000 USD. Therefore the index level of XYZ is:

$$
{XYZ}=\frac{(100*2000000*1.50)+(200*5000000*1.50)+(300*8000000*0.75)}{36000000} = 100
$$

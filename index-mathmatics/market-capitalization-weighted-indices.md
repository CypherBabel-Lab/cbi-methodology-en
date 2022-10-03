# Market Capitalization Weighted Indices

A majority of CBI’s crypto asset indices are market capitalization weighted and circulating-adjusted, where each crypto asset’s weight in the index is proportional to its total market value of its circulating supply. This is analogous to the free-float capitalization in the stock market.

CBI also provides capped versions of a market capitalization weighted index where single index constituents or defined groups of index constituents, such as sector or group, are confined to a maximum weight.

## Market Capitalization Weighted Index

Many of CBI’s indices are market capitalization weighted indices. Sometimes these are called value weighted or market cap weighted. A constituent's weight of a market capitalization weighted index is proportional to its market capitalization determined by its circulating supply.&#x20;

The index level of a market capitalization weighted index is calculated by:

$$
{Index Level}=\frac{{Index Value}}{{Divisor}}
$$

Where the numerator on the right hand side is the market value of an index with all constituents' circulating market capitalizations. This is summed across all the constituents in the index. The denominator is the divisor. If the numerator is US$ 1.0 trillion and the divisor is US$ 10 billion, the index level would be 100.

The _IndexValue_ is calculated by:

$$
{Index Value}={\sum_{i} P_{i} * Q_{i}}
$$

Where _P_ is the price of each constituent in the index, _Q_ is the quantity of each constituent's circulating supply, and _i_ denotes a constituent.

The weight of a constituent is calculated by:

$$
{W}_{i}=\frac{{P}_{i}*{Q}_{i}}{{Index Value }}
$$

Where _P_ is the price of the constituent _i_, _Q_ is the quantity of the circulating supply of the constituent _i,_ and _IndexValue_ is the market value of an index with all constituents' circulating market capitalizations.

{% hint style="info" %}
The real-time data of the price and quantity for the constituents in CBI indices are provided by well-established data aggregators, including CoinGecko and CoinMarketCap.&#x20;
{% endhint %}

### An example

Let's assume we are constructing a market capitalization weighted index named XYZ, which is composed of three constituents X, Y, and Z. The price and quantity of the circulating supply for each constituent are shown in the table:&#x20;

| Constituent | Price (US Dollar) | Quantity  |
| ----------- | ----------------- | --------- |
| X           | 100               | 2,000,000 |
| Y           | 200               | 5,000,000 |
| Z           | 300               | 8,000,000 |

We set the divisor as 36,000,000 USD, therefore the index level of XYZ is:

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

具上限市值加权指数（又称为具上限市值指数、具上限指数或具上限加权指数）是指对单一指数成分或指定的指数成分组别限定最大权重，超过的权重按比例在其余指数成分中分配的指数。随着成分价格的变动，其市值权重会改变，继而调整因子也会改变。因此具上限市值加权指数成分的权重需要不断进行重平衡，以确保满足上限规则。

具上限市值加权指数的总体计算方法与流通市值加权指数相同，由Index Value（指数值）和Dividor（指数除数）共同决定。具上限市值加权指数的计算方法为：

A capped market capitalization weighted index is one where single index constituents or defined groups of index constituents are confined to a maximum weight and the excess weight is distributed proportionately among the remaining index constituents. Sometimes, it is also called a capped market cap index, capped index or capped weighted index.&#x20;

As constituent prices move the weights will shift and the modified weights will change. Therefore, a capped market cap weighted index must be rebalanced from time to time to re-establish the proper weighting. The methodology for capped indices follows an identical approach to market cap weighted indices except that the indices apply an additional weight factor, or “AWF”, to adjust the float-adjusted market capitalization to a value such that the index weight constraints are satisfied. For capped indices, no AWF change is made due to corporate actions between rebalancings except for daily capped indices where the corporate action may trigger a capping. Therefore, the weights of stocks in the index as well as the index divisor will change due to notional market capitalization changes resulting from corporate events. The overall approach to calculate capped market cap weighted indices is the same as in the pure marketcap weighted indices; however, the constituents’ market values are re-defined to be values that will meet the particular capping rules of the index in question.

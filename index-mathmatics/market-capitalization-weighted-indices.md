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

Where _P_ is the price of constituent _i_, _Q_ is the quantity of circulating supply for constituent _i,_ and _IndexValue_ is the market value of an index with all constituents' circulating market capitalizations.


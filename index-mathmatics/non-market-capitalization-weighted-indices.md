# Non-Market Capitalization Weighted Indices

A non-market capitalization weighted index (also referred to as a non-market cap or modified market cap index) is one where the weights of the index constituents are not determined by the market capitalization weighted methodology. For example, the weights are user-defined. Between index rebalancing, most corporate actions generally don't affect index weights, as they are fixed. As the constituents' price move,  their weights will change accordingly. Therefore, a non-market capitalization weighted index must be rebalanced from time to time to reestablish proper weighting.

The overall approach to calculating non-market capitalization weighted indices is the same as the capitalization weighted indices. However, the constituents' market value are set to a value to achieve a specific weight at each rebalancing that is different from a purely circulating-adjusted market capitalization weighting.

The index level of a non-market capitalization weighted index is calculated by:

$$
{Index Level}=\frac{{Index Value}}{{Divisor}}
$$

The _IndexValue_ is calculated by:

$$
{Index Value}={\sum_{i} P_{i} * Q_{i}}
$$

Where the _IndexValue_ is the market value of an index with all constituents' circulating market capitalizations; _Pi_ is the price of each constituent in the index, _Qi_ is the quantity of each constituent's circulating supply, and _i_ denotes a constituent.

However, to calculate a non-market capitalization weighted index, the market value for each constituent in the index is redefined so that it has the appropriate weight in the index at the initial calculation date and also at each rebalancing date. The new adjustment factor used to establish the appropriate weighting is called Weight Adjustment Factor (WAF).&#x20;

Therefore, the constituent market value is calculated by:

$$
\text {CV}_{i}={P_{i} * Q_{i} * WAF_{i}}
$$

Where _CVi_ is the market value of constituent _i_, _Pi_ is the price of constituent _i_, _Qi_ is the quantity of the circulating supply of constituent _i,_ and W_AFi_ is the adjustment factor of constituent _i_.




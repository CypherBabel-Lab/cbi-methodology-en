# Divisor

The purpose of the index divisor is to maintain the continuity of an index level following the implementation of corporate actions, index rebalancing events, or other non-market-driven actions. And also, the index divisor is usually a smaller number than the index market value for people to read and process.

{% hint style="info" %}
The simplest capitalization weighted index can be thought of as a portfolio consisting of all available tokens of the constituents in the index. While one might track this portfolio’s value in US dollar terms, it would probably be a very large number – for example, the CIC55 circulating-adjusted market value might be a figure in the trillions of US dollars. Rather than deal with ten or more digits, the figure is scaled to a more easily handled number (e.g., 100). Dividing the portfolio market value by a factor, usually called the divisor, does the scaling.
{% endhint %}

An index is not exactly the same as an investment portfolio. For instance, when a constituent is added to or removed from an index, the index level should keep constant; while a portfolio’s value would usually change as tokens are swapped in and out. To assure that the index level does not change when constituents are added or removed, the divisor is adjusted to offset the change in the market value of the index. Thus, the divisor plays a critical role in the index’s ability to provide a continuous measure of market valuation when faced with changes to the constituents included in the index.&#x20;

In a similar manner, some corporate actions that cause changes in the market value of the constituents in an index should not be reflected in the index level. Adjustments are made to the divisor to eliminate the impact of these corporate actions on the index level.

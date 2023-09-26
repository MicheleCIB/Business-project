# Business-project
Task 1: perform a leaders &amp; follower analysis. Task 2: understand when some products/categories were popular in the past and define a popularity index to know every day which products are popular in order to activate marketing campaigns.
Preparing two different types of dataset, one for the leader and follower, one for the popularity index
For the leader and follower analysis we cretate a new dataset starting from the prices_competitor.csv,
adding market share and volatility columns For the popularity index we merged sales_data.csv
and stock_csv, then adding clicks_regular.csv and clicks_bidding.csv, finally we create the profit column.
From each one of this two new datasets we cretate 5 new datasets (one for each period) to conduct the analysis
To solve task 1, the leader and follower analysis for each period we decided to proceed like this: there are several
variables that can be taken into account depending on the context and objectives of the analysis. Some of the
common variables to consider include:
Market Share: the market share of a product or vendor can be an important indicator for identifying leaders and
followers. A high market share might indicate the dominance of a leader, while a lower market share might suggest
the presence of followers.
Sales volume: The sales volume of a product or seller can provide an indication of their popularity and success in
the market. Leaders tend to have a higher sales volume than followers.
Price: The price of a product or service can influence its position in the market. Leaders may have higher prices
than followers because of their reputation or the added value they offer.
Price volatility can also be an indicator of the dynamism and instability of a market. Leaders might have lower price
volatility, indicating greater stability and control over the market. On the other hand, followers might be subject to
larger and more unpredictable fluctuations in price, indicating a position of less control or influence.
In our case, we decided that the leader could be the one who has either the highest price, minimal price volatility
(less or equal to the mean of volatility for that period) or a fairly high market share (more than 15% of the total per
period).
Task 2
We combine all the values using different weights for the variables. Then we add the new values to the
respective dataframes. The first ones are for the q1, that doesn't have the number of bidding, the
remaining ones are for the the remaining periods and for the Black Friday.
We have chosen to determine the popularity index according to these criteria, using this weights;
Number of sales: represents the total number of units of a product sold during a certain time period.
A high number of sales indicates a higher popularity of the product. It corresponds to quantity.
Online search: Indicates how often the product is searched for on search engines or e-commerce
platforms. A high number of searches may indicate widespread interest in the product.
Profit: profit analysis can provide crucial information on the effectiveness of pricing strategies, the
profitability of the product and its popularity in terms of revenue generation. An increase in profits
may indicate an increase in demand or effective cost management, while a decrease in profits could
be a sign of declining popularity or fiercer competition.

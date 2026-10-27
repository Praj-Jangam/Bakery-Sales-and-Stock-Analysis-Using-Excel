Bakery Sales and Stock Analysis
Overview
This project analyses synthetic bakery sales and stock data across 14 Southampton-area shops for September 2026. I wanted to explore how sales and stale stock vary between shops and products, using a setting I’m familiar with through my work at Greggs.

The dataset contains 18,060 daily records covering 43 products. It includes a selection of products from different categories, rather than the full range sold in Greggs shops.

The data is synthetic: the figures were created for this project and do not represent actual Greggs sales, stock or shop performance.
Questions
The analysis focuses on three questions:
- How does estimated sales revenue compare across shops?
- Which products generate the most estimated revenue?
- How many items are recorded as stale across shops and products?
Dataset and Analysis
I created a synthetic dataset based on bakery shop operations. It includes daily records of products available, units sold, items sent to outlet and items recorded as stale. I used my experience in a bakery environment to help shape the product categories and stock patterns.

I used Excel to prepare and analyse the data:
- VLOOKUP matched product IDs to a separate price table.
- Revenue was calculated by multiplying units sold by the product price.
- SUMIF calculated total estimated revenue for each product.
- Pivot Tables compared revenue and stale quantities across shops.
- Filters and slicers helped explore selected products, shops and dates.
Challenges and Data Checks
Missing product price: When I used VLOOKUP to bring prices into the daily records, one product, Pigs in Blankets, returned an #N/A error. I checked the separate price table and found that the product was missing. I added its product ID and an example price to the table, which allowed the formula to find a match and calculate its estimated revenue.

Understanding stock differences: I calculated the difference between the quantity available and the quantities sold, sent to outlet and recorded as stale. Initially, I thought a positive difference meant stock was missing. On review, I realised that for products such as bottled drinks and crisps, it could include items still on the shelf.

The dataset does not record closing stock separately, so I did not treat these differences as confirmed losses.

I also checked for duplicate shop–product–date records and visible formula errors. None were found in the version reviewed.
Key Findings
To complete using the final Pivot Tables and product summary:
1. Shop revenue: 
2. Product revenue: 
3. Stale products: 
Limitations
The analysis covers a selection of products rather than the full Greggs product range. Some prices are example values, and revenue is estimated using units sold and product prices, so it does not account for discounts, meal deals or refunds.

Closing stock is not recorded separately, which means the stock difference cannot identify confirmed losses. The results describe the synthetic dataset and should not be used to judge actual shop performance.

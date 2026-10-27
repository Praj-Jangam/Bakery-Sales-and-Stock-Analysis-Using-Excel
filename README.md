# Bakery Sales and Stock Analysis Using Excel

## Overview

This project was inspired by my experience working at Greggs. I analysed a synthetic dataset in Excel to explore how sales and stale stock vary across 14 Southampton-area shops and different products during September 2026.

The dataset contains 18,060 daily records covering 43 products. It includes a selection of products from different categories rather than the full Greggs range.

"The figures were created for this project and do not represent actual Greggs sales, stock or shop performance."

## Questions

The analysis focuses on three questions:

- How does estimated sales revenue compare across shops?
- Which products generate the most estimated revenue?
- How many items are recorded as stale across shops and products?

## Dataset and Analysis

I created a synthetic dataset based on bakery shop operations. It includes daily records of products available, units sold, items sent to outlet and items recorded as stale. I used my experience in a bakery environment to help shape the product categories and stock patterns.

I used Excel to prepare and analyse the data:

- **VLOOKUP** matched product IDs to a separate price table.
- **Revenue** was estimated by multiplying units sold by the product price.
- **SUMIF** calculated total estimated revenue for each product.
- **Pivot Tables** compared revenue and stale quantities across shops.
- **Filters and slicers** helped explore selected products, shops and dates.

## Challenges and Data Checks

**Missing product price:** When I used VLOOKUP to bring prices into the daily records, one product, Pigs in Blankets, returned an #N/A error. I checked the separate price table and found that the product was missing. I added its product ID and an example price to the table, which allowed the formula to find a match and calculate its estimated revenue.

**Understanding stock differences:** I calculated the difference between the quantity available and the quantities sold, sent to outlet and recorded as stale. Initially, I thought a positive difference meant stock was missing. On review, I realised that for products such as bottled drinks and crisps, it could include items still on the shelf.

The dataset does not record closing stock separately, so I did not treat these differences as confirmed losses.

I also checked for duplicate shop-product-date records and visible formula errors. None were found in the version reviewed.

## Key Findings

- **Shop revenue:** Hedge End, R1 Hedge End TP, Tollbar had the highest estimated revenue, at £76,038.00.
- **Product revenue:** Sausage rolls generated the highest estimated product revenue, at £73,932.75 across all shops.
- **Stale products:** Southampton, Adanac Pk Drive Thru recorded the highest total of stale products, at 1,166 units.

These figures cover September 2026 and reflect the synthetic dataset.

## Limitations

The analysis covers a selection of products rather than the full Greggs product range. Some prices are example values, and revenue is estimated using units sold and product prices, so it does not account for discounts, meal deals or refunds.

Closing stock is not recorded separately, which means the stock difference cannot identify confirmed losses. The results describe the synthetic dataset and should not be used to judge actual shop performance.

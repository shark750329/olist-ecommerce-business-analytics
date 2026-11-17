# olist-ecommerce-business-analytics
Project Overview
A comprehensive, end-to-end analytics deep dive into the Brazilian Olist e-commerce marketplace, synthesizing commercial performance, basket economics, payment workflows, logistics stages, and unstructured Portuguese review data into an evidence-based decision framework.

Scope: 99,441 Orders | 96,096 Unique Customers | 32,951 Catalog SKUs | 3,095 Sellers | R$ 13.59M Merchandise Revenue

🎯 Core Strategic Diagnosis
Olist's expansion is almost entirely acquisition-driven rather than monetization-driven. Because weighted Average Order Value (AOV) grew by only +0.92% (R
135.56
→
R
135.56→R 136.80) while revenue grew 137.22% (like-for-like Jan–Aug 2017 vs 2018), sustaining growth requires shifting focus from raw order volume to basket expansion, fulfillment reliability, and repeat retention.

📊 Key Performance Indicators
Metric	Value
Total Orders	99,441
Orders with Items	98,666
Unique Customers	96,096
Catalog SKUs	32,951
Active Sellers	3,095
Merchandise Revenue	R$ 13,591,643.70
Platform AOV	R$ 137.75
Total Payment Value (incl. freight)	R$ 16,008,872.12
Total Freight	R$ 2,251,909.54
Freight-to-Revenue Ratio	16.58%
Repeat Purchase Rate	3.12% (2,997 customers)
Delivery Success Rate	97.02% (96,478 orders)
🔍 Analysis Modules
1. Executive Storyline & Macro Growth Trajectory (2016–2018)
+135.07% order volume growth (Jan–Aug 2017 vs 2018)

+137.22% merchandise revenue growth over the same matched window

Historic Black Friday spike: 7,544 orders (Nov 2017, +2,913 MoM)

Note on partial data-capture windows (Sep/Oct 2018 cutoff)

2. Demand Concentration & Volume-AOV Matrix
Top 5 categories: 39.90% of orders

Top 10 categories: 62.93% of orders / 63.19% of revenue

Top 20 categories: 88.31% of orders / 85.13% of revenue

Trade-off analysis: Computers AOV (R 1,231.84) is 8.6× *Health & Beauty* (R 142.45), yet Health & Beauty generates 5.6× more total revenue

3. Catalog Productivity & Customer Retention Economics
96.88% of customers (93,099) placed only 1 order

Only 3.12% (2,997) ever returned

Catalog productivity leader: Watches & Gifts — ~R 907 revenue per listed SKU (1,329 SKUs) vs *Furniture & Decor* at ~R 275 (2,657 SKUs)

4. Basket Size Architecture & Multi-Item Purchasing
Platform average basket: 1.14 items/order

90.06% single-item orders; 99.02% contain ≤3 items

Top multi-item categories: Furniture & Decor (19.09%), Office Furniture (18.07%), Garden Tools (15.58%)

Multi-item orders lift category AOV by 18%–29% above single-item prices

5. Payment Ecosystem & Approval Delay Bottleneck
Credit Card: 78.34% of transaction value (R$ 12.54M), avg 3.51 installments

Boleto: 17.92% (R$ 2.87M) — but accounts for 57.1% of >24h approvals

Overall Stage 1 (Purchase → Approval) mean: 10.42 hours

15.17% of orders suffer ≥25-hour approval delays

Delay risk rises monotonically with basket size (10.3h at 1 item → 27.6h at 8 items)

6. Freight Economics & Seller Supply Concentration
Platform freight-to-revenue ratio: 16.58%

Furniture & Decor: 23.67% freight/revenue (bulky items erode margin)

Computers: only 4.0% freight/revenue (high ticket absorbs shipping)

São Paulo (SP): 70.77% of orders from 59.74% of sellers (ratio 1.18)

Under-indexing states: PR (0.69), SC (0.60), RJ (0.79), RS (0.48)

7. Fulfillment Pipeline & the "NULL Category" Discovery
97.02% delivered; 1.74% in-flight; 1.24% lost/failed

Critical anomaly: NULL-category orders (2,248) = 28.75% of all cancellations and 99.01% of all unavailable orders

Data governance rule: Never silently drop NULL categories via inner joins

8. Physical & Geographic Drivers of Delivery Delays
Weight penalty: +37.41% delivery time for 25–49 kg orders vs 0–4 kg baseline

Macro-geography overwhelms physical weight at state grain:

SP: 8.72 days avg (2.04 kg)

RR: 28.23 days (1.76 kg)

AP: 28.21 days (1.85 kg)

Priority logistics hotspots: RJ destination, MA × Health/Beauty origin, MG × Garden Tools

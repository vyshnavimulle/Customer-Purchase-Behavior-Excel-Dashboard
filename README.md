# Customer Purchase Behavior Analysis - Retail Fashion (Excel Dashboard)

## Business Problem
A retail fashion company wants to understand customer purchase behavior to improve marketing, inventory planning and product recommendations. This project answers:
- Which customer segments bring the most revenue?
- How do product categories, seasons and purchase frequency affect sales?
- How do shipping type, discounts and promo codes affect purchases?
- What do customers prefer by payment method and subscription status?

## Objective
An end-to-end Excel analysis: data loading, cleaning, preprocessing, an interactive dashboard (PivotTables, PivotCharts, slicers) and business insights.

## Dataset
- File: `raw-data/shopping_behavior_updated.csv`
- 3,900 customer purchases and 18 columns (Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount (USD), Location, Size, Color, Season, Review Rating, Subscription Status, Shipping Type, Discount Applied, Promo Code Used, Previous Purchases, Payment Method, Frequency of Purchases)

## Tools and Skills
Microsoft Excel | Data Cleaning | Data Preprocessing | PivotTables | PivotCharts | Slicers | Dashboard Design | Business Insights

## Workflow
1. **Data loading:** imported the CSV into Excel and verified column names, data types and structure.
2. **Data cleaning:**
   - Checked text fields (Location, Size, Color, Season) for spaces, typos and mixed case
   - Checked numeric fields (Age, Purchase Amount, Previous Purchases, Review Rating)
   - Checked Yes/No fields for uniform values
   - Merged duplicate frequency labels (Bi-Weekly into Fortnightly, Every 3 Months into Quarterly)
   - Checked duplicates on Customer ID + Item Purchased (none found)
   - Converted the data to an Excel Table named `PurchaseData`
3. **Data preprocessing:** created Age Group (Young 25 or below, Adult 26-50, Senior above 50), Revenue, Subscription Flag (1/0) and Rating Rounded (whole stars).
4. **Dashboard:** built 9 PivotTable/PivotChart views, added summary cards and slicers (Season, Gender, Category).
5. **Insights:** analyzed patterns from the dashboard.

## Summary Numbers
| Total Revenue | Total Purchases | Average Purchase | Average Rating | Subscribed Customers |
|---|---|---|---|---|
| $233,081 | 3,900 | $59.76 | 3.75 | 27% |

## Key Insights
- **Category:** Clothing brings the most revenue (45%), followed by Accessories (32%), Footwear (15%) and Outerwear (8%).
- **Season:** Revenue is almost evenly spread across the four seasons (24% to 26%), with Fall slightly ahead.
- **Age and gender:** Adults (26-50) contribute 47% of revenue, Seniors 38% and Young customers 15%. Male customers account for about 68% of purchases and revenue, so the female customer base is much smaller.
- **Purchase frequency:** Quarterly (29.5%) and Fortnightly (28%) shoppers bring nearly 58% of revenue.
- **Shipping and payment:** All shipping types and payment methods bring similar revenue (about 16% to 17% each), so no single option dominates.
- **Discounts:** 57% of revenue came from purchases without a discount. The average purchase is about the same with a discount ($59.28) and without one ($60.13).
- **Ratings:** Most ratings fall between 3 and 4 stars.
- **Loyalty:** Customers with more previous purchases do not spend noticeably more per purchase.

## Recommendations
- Focus marketing and stock planning on Clothing and Accessories.
- Target the 26-50 age group and grow the female customer base.
- Reward regular Quarterly and Fortnightly shoppers with loyalty offers.
- Review discount offers, since customers spend about the same with or without them.

## Data Notes
- In this dataset, Discount Applied and Promo Code Used contain the same Yes/No values, so both charts show identical numbers.
- Review ratings were rounded to whole stars for the distribution chart. The lowest original rating is 2.5.

## Repository Structure
- `raw-data/` original dataset
- `excel-files/` complete workbook (Raw_Data, Clean_Data, pivot sheets P1 to P9 and the Dashboard)
- `screenshots/` dashboard images

## Author
Mulle Vyshnavi | linkedin.com/in/vyshnavi-mulle

## Acknowledgements
Thanks to my trainer Vineela Diddi, my mentor Bhargav Kunapareddy and Innomatics Research Labs for their guidance and support.

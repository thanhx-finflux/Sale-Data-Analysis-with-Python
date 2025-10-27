# Sale-Data-Analysis-with-Python
This project analyzes sales and customer data using Python, Pandas, Matplotlib, Seaborn, and Plotly. The Jupyter notebook provides insights into sales performance, customer demographics, profitability, discounts, and more, accompanied by visualizations and actionable recommendations.

## Overview
This analysis uses sample datasets of customer and sales data to uncover trends, including:
- Data clearing and exploration with missing values and duplicates.
- Merge customer and sales data for deeper insights.
- Aggregations by category, sub-category, region, ship mode, and customer segments.
- Visualizations such as bar charts, scatter plots for sales, profits, quantities, and discounts.
- Statistical tests (T-test, ANOVA test)
- Insights on high/low profit products, discount strategies, and inventory recommendations.

  The goal is to provide data-driven recommendations for optimizing marketing, inventory, and pricing strategies.
  ## Features
  - Data processing: Load, clean, and merge CSV datasets using Pandas.
  - Exploratory Data Analysis (EDA): summary statistics, missing value checks, and data info.
  - Visualizations: Interactive plot with Plotly
  - Key insights:
    -  Profitability by category/sub-category
    -  Discount impacts on sales and profits.
    -  Regional and demographic trends
    -  Product performance (top/bottom products by profit)
  -  **Recommendations:** Implement strategies that focus on high-profit items, methods for mitigating losses, and conducting A/B testing for discounts.
 
## Prerequisites:
- Python 3.12+: with libraries (pandas, numpy, matplotlib, seaborn, plotly, scipy)
- Jupyter notebook
## View Dynamic Plotly Graphic on Google Colab

[Google Colab](https://drive.google.com/file/d/1PBEWV2AvE5UqhhhfCkdNZ7I0Diw-Kw4R/view?usp=sharing)

## Visualizations:

Total Sales and Profit by Category

<img width="800" height="600" alt="Image" src="https://github.com/user-attachments/assets/675bb17c-665a-4e3e-8a25-cf4314823bd4" />

Total Sales vs Profit with sub-categories

<img width="1400" height="1000" alt="Image" src="https://github.com/user-attachments/assets/53c7eff3-64c6-4927-92cf-0f4e53400622" />

<img width="1400" height="1000" alt="Image" src="https://github.com/user-attachments/assets/620fe7b7-9181-41f8-85e7-ccbc25ca908a" />

<img width="1400" height="1000" alt="Image" src="https://github.com/user-attachments/assets/b2eb90ff-5897-492a-866b-888164ab473e" />

Total Profit vs Quantity by Sub-Category

<img width="1400" height="1000" alt="Image" src="https://github.com/user-attachments/assets/477a9630-185a-4000-b661-f63ce698a069" />

```
### Key Observations
- Phone high quantity and very high profit, this sub-category is a clear profit driver.
- Chairs have a high quantity, but profit is much lower compared to phones, which presents an opportunity to improve profit margin on chairs.
- Tables quantity but negative profit, need to investigate reasons for losses and consider strategies to improve profitability or discontinue. This is a red flag for the business, even though sales are high. They are losing money on this sub-category.
- Binders and Paper: high quantities sold but relatively modest profit, opportunity to optimize pricing or cost structure to boost profitability.
- Copiers have  low quantity but very high profit, focus on marketing and sales efforts to maximize revenue from this sub-category. This is a premium product with a high profit margin.
- Accessories, Storage, and Furnishings are mid-tier items with moderate quantities and profits; these are steady contributors to overall profitability.
- Fasteners, Envelopes, Art, and Machines, with low quantities and low profits, may not warrant significant focus but should be reviewed periodically to ensure they do not negatively impact overall profitability.
- Books' negative profit should be carefully analyzed to identify reasons for losses and consider strategies such as price adjustments, cost reductions, or discontinuation if profitability cannot be improved.
### Key Recommendations
- Focus on Phones and Copiers as key profit drivers.
- Investigate and address losses in Tables, Supplies, and Books sub-categories.
- Optimize Chairs has good sales volume but a weaker profit margin. Explore pricing or cost strategies to boost profitability.
- Leverage Binders and Paper for steady revenue, while monitoring mid-tier items for sales trends.
- Reassess low performers like Fasteners, Envelopes, Art, and Machines may not justify significant focus, heavy marketing, or inventory efforts.
```
Scatter plot average profit vs average discount with sales size by sub-category

<img width="1400" height="1000" alt="Image" src="https://github.com/user-attachments/assets/0d7d63a8-56ad-4825-90df-19f0c4eb876e" />

```
### Key Observations
- Copiers' profit is very high (55617.90), low quantity sold (234), discount at 16% is a high margin product, but low sales volume.
- Phone's profit is high (44516.25), high quantity sold (3289), discount at 15% good balance of volume and margin. Strong balance of sales and profit.
- Accessories profit is good (41936.78), high quantity sold (2976), discount at 8% solid performer. A healthy margin product with good sales volume.
- Paper profit is good (34053.34), very high quantity sold (5178), discount at 7.5% high volume, low margin product. A volume driver with solid profit contribution.

=> These are profit drivers for the business.

- Binders' profit is good (30221.64), very high quantity sold (5974), discount at 37% very high discount to drive volume, but still profitable. The high discount strategy is working here. It is heavily discount-driven. Without a discount, it may be loss-making.
- Chair's profit is moderate (26590.15), high quantity sold (2356), discount at 17% opportunity to improve margin on good sales volume.

=> These are volume drivers but discount-sensitive. Test smaller discounts to see demand impact.

- Storage profit is moderate (21279.05), high quantity sold (3158), discount at 7.5% solid performer.
- Furnishings profit is moderate (13059.25), moderate quantity sold (3563), discount at 14% steady contributor.
- Appliances profit is moderate (18138.07), moderate quantity sold (1729), discount at 16% steady contributor.
- Art profit is low (6527.96), moderate quantity sold (3000), discount at 7.5% low performer.

=> These categories sell decently but are not major profit contributors. Monitor for trends; they may need to optimize costs or bundle with other products to boost sales.

- The table's profit is negative (-17725.59), a moderate quantity was sold (1241), and a discount of 26% needs to be investigated to determine the reasons for the losses and consider strategies to improve profitability or discontinue.
- Book's profit is negative (-3472.56), low quantity sold (868), discount at 21% need to investigate reasons for losses and consider strategies to improve profitability or discontinue.
- Supplies profit is negative (-1188.99), low quantity sold (647), discount at 7.5% need to investigate reasons for losses and consider strategies to improve profitability or discontinue.

=> These are loss-making sub-categories that require immediate attention. Analyze cost structure, pricing, and demand to identify improvement strategies or consider discontinuation. The problems here could be high costs, low prices, or insufficient demand.

- Feasters, Labels, Evenlopes, and Machines have low profit but are not loss-making, with moderate to low quantity sold. These may not warrant significant focus, but should be reviewed periodically to ensure they do not negatively impact overall profitability.
### Key Recommendations
- Protect Stars: Focus on maximizing sales and marketing efforts for Copiers, Phones, Accessories, and Paper to leverage their substantial profit and sales performance. Keep low discounts, invest in supply chain efficiency to maintain healthy margins.
- Optimize Cash Cows: Review discount strategies for Binders and Chairs to improve profit margins without significantly impacting sales volume. Experiment with lower discounts to find the optimal balance.
- Monitor Steady Contributors: Keep an eye on Storage, Furnishings, Appliances, and Art for any changes in sales trends. Consider bundling or promotional strategies to boost their performance.
- Address Loss-Makers: Conduct a thorough analysis of Tables, Books, and Supplies to identify the root causes of losses. Explore options such as price adjustments, cost reductions, or discontinuation if profitability cannot be improved.
- Review Low Performers: Periodically assess Fasteners, Labels, Envelopes, and Machines to ensure they do not negatively impact overall profitability. Consider phasing out if they consistently underperform.
```

```
In summary, the profit analysis highlights the need to focus on high-performing sub-categories while addressing the challenges faced by loss-making items. Strategic adjustments in pricing, discounting, and marketing can help optimize overall profitability.
### Discount Analysis
- The discount analysis reveals significant variations in discount strategies across states, ship modes, product categories, age groups, and profit/loss outcomes. These insights can inform targeted discounting approaches to enhance sales performance while maintaining profitability. The category and sub-category analyses provide actionable recommendations for optimizing inventory management, marketing strategies, and overall business performance.
### Key Findings
- States like Arkansas, Oregon, and Colorado offer higher average discounts, while states like Maryland and Oklahoma have lower discounts.
- First Class and Standard Class ship modes have higher average discounts compared to Second Class.
- Furniture category has the highest average discount, while Technology has the lowest.
- Loss-making transactions have significantly higher average discounts compared to profitable ones.
- Younger age groups (18-30 and 31-45) tend to receive slightly higher discounts compared to older age groups (46-60 and 61+).
## Summary of Findings
Overall, the discount analysis reveals significant variations in discount strategies across states, ship modes, product categories, age groups, and profit/loss outcomes. These insights can inform targeted discounting approaches to enhance sales performance while maintaining profitability. The category and sub-category analyses provide actionable recommendations for optimizing inventory management, marketing strategies, and overall business performance. Profitability is strongly influenced by product category and subcategory, while customer demographics such as age, segment, ship mode, and region have a lesser impact.
### Suggested Next Steps
- Further investigate the impact of discounts on sales volume and profitability to refine discount strategies.
- Explore customer feedback and preferences regarding discounts to better tailor offerings.
- Conduct A/B testing of different discount strategies to identify the most effective approaches.
- The discount distributions vary significantly across different ship modes.
The ship modes with the highest average discounts are First Class (16.46%) and Standard Class (16.00%), while Second Class has the lowest average discount (13.89%). The ANOVA test confirms that these differences are statistically significant (p-value < 0.05). This insight can help optimize shipping strategies to balance cost and customer satisfaction.
- The first class and standard class ship modes offer higher discounts, possibly to attract customers and offset higher shipping costs.
- Negative profit items like Tables, Supplies, and Books should be carefully analyzed to identify reasons for losses. Consider strategies such as price adjustments, cost reductions, or discontinuation if profitability cannot be improved. Review pricing strategies, source alternatives, and marketing approaches to mitigate losses.
- High profit-low quantity items like Copiers should be prioritized for marketing and sales efforts to maximize revenue.
- High profit-high quantity items like Paper, Accessories, Phones, and Binders should be stocked adequately to meet demand and capitalize on their profitability. Prioritize promotions, discounts, and advertising campaigns. Ensure sufficient inventory levels to avoid stockouts, and explore cross-selling opportunities with related products.
- Mid-Tier items like Chairs, Furnishings, Appliances, and Storage should be monitored for sales trends and adjusted inventory levels accordingly. Consider bundling with high-profit items to boost sales.

```
### Contact

Thanh Xuyen, Nguyen

LinkedIn: [xuyen-thanh-nguyen-0518](https://www.linkedin.com/in/xuyen-thanh-nguyen-0518/)

Email: thanhxuyen.nguyen@outlook.com

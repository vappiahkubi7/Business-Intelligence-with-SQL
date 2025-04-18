# BUSINESS INTELLIGENCE WITH SQL: SALES & INVENTORY INSIGHTS FOR KWABS INC.

> Transforming Raw Data into Strategic Decisions for a Multi-State Retail Brand

---

![living-room-728731_1280](https://github.com/user-attachments/assets/a10b7fa8-2af3-4fa0-8c29-e10c0ab40038)


## PROJECT OVERVIEW

In today’s competitive retail environment, businesses must move beyond raw data to derive **actionable insights**. This project demonstrates how SQL can power **end-to-end analysis** of sales trends, product performance, and customer behavior for **Kwabs Inc**, a furnishings and office supplies retailer operating across the United States. 

As the company scales, understanding product performance, regional sales distribution, and customer ordering patterns becomes critical for operational efficiency and long-term success. This project uses SQL to uncover trends that inform **inventory optimization**, **category management**, and **strategic pricing decisions**.

---

![istockphoto-2049950886-612x612](https://github.com/user-attachments/assets/24cc7893-8e89-47ae-aaba-3f569d4720da)

## PROJECT OBJECTIVES

- Analyze sales performance across product categories including furnishings, public areas, and office supplies.  
- Identify high-performing and underperforming products to support smarter inventory management.  
- Evaluate customer ordering trends across different properties and geographic regions.  
- Use SQL queries and visualizations to compare year-over-year sales performance.  
- Translate insights into **data-driven business recommendations** to improve profitability.

---

## SKILLS & CONCEPTS DEMONSTRATED 

- **Business Understanding**: Grasping Kwabs Inc's operational landscape and objectives  
- **Data Exploration**: Evaluating datasets for relevance and analytical potential  
- **Data Extraction**: Retrieving key fields from `Orders`, `Products`, and `PropertyInfo` tables  
- **SQL Analysis**: Using SQL to calculate KPIs, segment pricing tiers, and analyze trends  
- **Strategic Thinking**: Providing actionable business recommendations based on findings  

---

## SQL TECHNIQUES 

To derive actionable insights from the dataset, the following SQL methods were employed to transform raw data into structured business intelligence:

- Data Integration with JOINS: Seamlessly connected the Products, Orders, and PropertyInfo tables using inner joins, creating a unified dataset that reflects the full sales journey—from product details and purchase behavior to property-level context.

- Key Metric Derivation via AGGREGATES: Leveraged SQL aggregate functions like SUM(), AVG(), and COUNT() to compute essential performance indicators such as total units sold, average product prices, and category-level sales—providing a foundation for performance tracking and trend analysis.

- Targeted Data Exploration with FILTERS: Applied precise WHERE clauses to isolate meaningful subsets of data, enabling focused analysis on specific years, categories, or price tiers. This allowed for in-depth exploration of patterns and outliers.

- Data Segmentation with GROUPING: Used GROUP BY to segment the data across meaningful dimensions like year, state, and product category. This segmentation facilitated comparative analysis across time and business segments, enhancing the depth of insights generated.

- Insight Extraction through Strategic Query Design: Crafted modular, layered SQL queries that enabled drilling down from macro-level trends to micro-level details, supporting business decisions on pricing, inventory, and customer targeting.

| Technique         | Purpose |
|------------------|---------|
| `JOIN`           | Merging data across tables (`Orders`, `Products`, `PropertyInfo`) |
| `GROUP BY`       | Summarizing metrics by category, region, or year |
| `CASE`           | Creating custom segments (e.g., price classification) |
| Aggregations     | Using `SUM()`, `AVG()`, `COUNT()` for key performance metrics |
| Filtering        | Targeted analysis using `WHERE`, `HAVING` |
| Subqueries       | Refining logic for more complex insights |

---

## DATA MODELLING: ENTITY-RELATIONSHIP DIAGRAM (ERD)

To ensure a clear understanding of the database structure and relationships, I utilized an Entity-Relationship Diagram (ERD) to map out the logical schema. This visual representation provided a high-level overview of how data entities interact, supporting the development of efficient and accurate queries.

The ERD highlights the core architecture of the dataset, which is built around three main tables:
- `Orders`
- `Products`
- `PropertyInfo`
  
These entities are linked through primary and foreign key relationships, forming a relational model that supports seamless data integration.

By laying out how information flows between orders, products, and customer property data, the - ERD:
- Clarifies data dependencies and constraints
- Enhances understanding of data normalization and referential integrity
- Serves as a blueprint for designing SQL queries that reflect real-world business logic

This structured approach ensures that analytical outcomes are both technically sound and aligned with business objectives, enabling Kwabs Inc to draw deeper insights into sales dynamics, customer distribution, and inventory management strategies.

![image](https://github.com/user-attachments/assets/118dc6cd-7c69-4949-912f-1ca6f3d09f5a)

---

## DATA ANALYSIS SNAPSHOT

### Unified Order View
This query consolidates critical data from the Orders, Products, and PropertyInfo tables to deliver a single, integrated view of sales transactions. It combines product details, pricing, quantities, and property locations into one cohesive dataset. This unified structure supports comprehensive analysis of customer purchasing patterns, category performance, and regional sales activity—empowering Kwabs Inc to make informed, strategic decisions based on complete order-level insights.

![image](https://github.com/user-attachments/assets/1a12e062-0c60-498a-bf21-4e030f16c0ed)


### Geographic Distribution
This query returns the list of cities and states where Kwabs Inc operates, showing a presence across 20 U.S. states. By mapping the geographic distribution of its properties, the analysis offers valuable insight into market coverage and regional reach—supporting smarter, location-specific strategies for inventory planning, marketing, and sales optimization.

![image](https://github.com/user-attachments/assets/bf3ee8a3-8c32-4031-ba57-f3988f7ef26f)


### Product Categories
This query outlines the range of product categories carried by Kwabs Inc, revealing five unique groupings. Understanding this classification supports deeper analysis of inventory strategy, helps assess the balance across product lines, and serves as a foundation for evaluating category-specific performance and future growth opportunities.

![image](https://github.com/user-attachments/assets/2d873bd4-f5aa-434a-b89d-d048e40937f7)


### Product Count by Category
This query summarizes the number of products within each category offered by Kwabs Inc. The results show that Furnishings has the largest selection with 26 products, while Office Supplies has the fewest at 13. This breakdown reveals how inventory is allocated across categories, offering key insights that can inform restocking strategies, product prioritization, and adjustments to better align inventory with demand trends.

![image](https://github.com/user-attachments/assets/ee6890bb-0915-4480-ae4d-1c0366d1b18b)


### Highest & Lowest Priced Products
This query identifies the top five highest- and lowest-priced products in Kwabs Inc’s catalog. The King Bed emerges as the most expensive item at $300, followed by the Double Bed, while low-cost essentials like Washcloth, Flyer Holder, and Paper Clips are priced at $3 each. This contrast provides a clear view of the product pricing spectrum, supporting strategic decisions around pricing tiers, promotional efforts, and the balance between premium and budget-friendly offerings.

![image](https://github.com/user-attachments/assets/368ba803-0ee2-4181-810a-97c966ebf99d)


### Average Price by Category
This query examines the average product price across each category, uncovering key pricing trends. Furnishings leads with the highest average price at $83.65, indicating a strong presence of high-value items, followed by Public Areas. In contrast, Office Supplies has the lowest average price at $22.69, reflecting its focus on low-cost, high-frequency products. This insight into pricing distribution helps assess product value across segments and supports strategic decisions in pricing optimization, product positioning, and inventory planning.

![image](https://github.com/user-attachments/assets/9cf2b19e-b5a9-4b3b-bb9c-141885ca2aed)


### High-Value Product Filter
This query isolates products priced over $200, uncovering four premium items—King Bed, Double Bed, Leaf Blower, and Sofa. Highlighting these high-ticket products offers a focused view into the upper tier of the inventory. These insights can inform premium pricing strategies, targeted promotions, or bundled offers, helping Kwabs Inc maximize returns on high-margin products.

![image](https://github.com/user-attachments/assets/d365f0ab-22d8-4377-b06d-a35b62b51e3f)


### Year-Over-Year Sales Comparison
This query summarizes the total quantity of products ordered in 2015 and 2016, showing a modest rise from 5,015 units to 5,081 units. While the growth is slight, it signals a positive shift in demand. This trend offers a foundational view of sales momentum and can be leveraged to inform inventory forecasting, capacity planning, and annual performance evaluation.

![image](https://github.com/user-attachments/assets/b99969c2-ad41-4913-8f65-258f020b1227)


### Price Segmentation
This query evaluates whether a product's price is more than $200, creating a new column that indicates if a product is "Above 200" or "Below or Equal to 200." The results reveal that only 4 products out of 94 product categories fall into the "Above 200" category, while the majority are priced "Below or Equal to 200." This classification provides a clear view of the distribution of high-value versus more affordable products, aiding in pricing strategy and product segmentation.


![image](https://github.com/user-attachments/assets/37140c11-07ec-4bd1-9dea-8eef1865adda)

---

## STRATEGIC RECOMMENDATION

### 1. **Leverage High-Value Products**
Premium products such as the King Bed, Double Bed, Leaf Blower, and Sofa, though fewer in number, have significant revenue potential due to their higher price points.

🔹 Action Plan:
- Design targeted marketing campaigns that highlight these products.
- Introduce upsell or bundle strategies to enhance average order value.
- Position them prominently in both physical and digital sales channels to maximize visibility and conversions.

### 2. **Optimize High-Demand Categories**
The Furnishings category stands out with both the highest average price and the largest product count. This indicates strong customer demand and substantial revenue contribution.

🔹 Action Plan:
- Ensure consistent stock availability to avoid missed sales.
- Explore adding more variety or complementary items within the category.
- Consider seasonal or trend-based expansions aligned with customer behavior.

### 3. **Rework Low-Margin Segments**
The Office Supplies category has the lowest average price, which often translates into lower profit margins. However, it holds potential through volume and creative packaging.

🔹 Action Plan:
- Introduce product bundles to encourage higher cart values.
- Offer subscription models for repeat-purchase items (e.g., paper, clips).
- Test value-added services or loyalty rewards tied to office essentials.

### 4. **Capitalize on Sales Trends**
The modest growth from 5,015 units in 2015 to 5,081 units in 2016 suggests a steady upward trend in product demand.

🔹 Action Plan:
- Use historical data to enhance demand forecasting and reduce overstocking.
- Align marketing and inventory planning with identified seasonal patterns.
- Monitor product velocity by region and time to sharpen decision-making.

### 5. **Double Down on High-Performing Regions**
With properties in 20 U.S. states, Kwabs Inc has a wide geographical footprint. Certain regions are likely outperforming others.

🔹 Action Plan:
- Segment performance by region to identify top markets.
- Invest in localized marketing, regional promotions, and logistics enhancements.
- Consider opening distribution hubs or expanding presence in high-performing zones.

### 6. **Revamp or Replace Poor Performers**
Categories or products showing low movement or interest should be evaluated for their contribution to revenue and relevance to customers.

🔹 Action Plan:
- Audit slow-moving SKUs and determine if they need repositioning, bundling, or retiring.
- Test new products aligned with category gaps or emerging trends.
- Reallocate shelf space and marketing focus to more promising inventory segments.

### 7. **Implement Ongoing Price Reviews**
Price-based segmentation revealed that only 4 out of 94 products fall above the $200 threshold. This insight can fuel a dynamic pricing model.

🔹 Action Plan:
- Regularly review pricing tiers using the “Above 200” vs. “Below or Equal to 200” model.
- Re-evaluate pricing based on category performance, customer sensitivity, and competition.
- Align promotional strategies with pricing tiers to capture different customer segments.

---

## CONCLUSION

This project illustrates how **SQL-powered data analysis** can provide deep insights into business performance. With actionable metrics across inventory, sales, and customer geography, Kwabs Inc can make confident, **data-driven decisions** to drive growth and profitability.

---

> ⚠️ **Disclaimer:**  
*All data, reports, and insights presented in this repository are entirely fictional and used for educational or demonstration purposes only. They do **not** contain any proprietary, confidential, or sensitive information from any actual company, institution, or individual. Any resemblance to real entities or data is purely coincidental.*


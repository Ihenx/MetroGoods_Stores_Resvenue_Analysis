# MetroGoods Stores Sales Analysis
## Introduction
The sales dashboards developed for MetroGoods Stores provide a comprehensive overview of business performance across key dimensions such as sales, customers, product categories, and demographics. They help address essential business questions around sales trends, customer behavior, and profitability. This report summarizes the insights gained from the dashboards and how they relate to MetroGoods’ business objectives.

## Business Questions Addressed
The MetroGoods Sales Analysis project was designed to answer the following key business questions:
* Which product categories generate the highest total sales and revenue? 
*  What are the peak sales months, and how do they compare to low-performing months? 
* Which customer demographic segments (age group, gender) spend the most? 
* What is the average purchase amount per transaction and per customer?
* Which specific product categories are top sellers and which are underperforming?

  ## Who are the stakeholders?
* Sales Department – to identify high- and low-performing Product Categories and
boost overall sales.
* Finance Department – to track revenue, average purchase values, and
profitability.
* Operations Management –Which includes the CEO to allocate resources effectively across stores and
peak sales periods.


## What insights will help solve the problem?
### Sales trends over time (monthly and seasonal performance):
Understanding how sales fluctuate month-to-month and across different seasons
will help MetroGoods identify peak demand periods and slow months

### Customer demographic insights (age and gender):
Analyzing purchase patterns by demographic groups reveals who the key
customers are and what they prefer.

###  Category-level performance to inform marketing focus and stock management:
Evaluating the performance of different product categories (e.g., Electronics,
Clothing, Beauty) allows management to see which categories are driving
revenue and which may need a different approach.
  ## Dataset Overview
### 📂 Dataset Description  

The **MetroGoods Stores dataset** contains the following columns:  

| Column        | Description                                           |
|---------------|-------------------------------------------------------|
| **Date**      | Records the transaction date                          |
| **Category**  | Indicates the product category                        |
| **Gender**    | Represents the customer’s gender                      |
| **Price**     | Unit price of the item purchased                      |
| **Quantity**  | Number of units sold                                  |
| **Total Amount** | Overall revenue generated (`Price × Quantity`)     |



  ## Data Cleaning
  **Tool Used: Power Query**
  
  <img width="1915" height="1034" alt="image" src="https://github.com/user-attachments/assets/1aeaef58-2449-492d-b643-ec13648e7078" />

 ### Steps Performed
1. Renamed Column <br>
**Action:** Changed the column name  Amount to  Sales.<br>
**Reason:** To provide a clearer and more accurate description of the data stored in the column. <br>
2. Standardized Date Format <br>
**Action:** Converted the Date column format from Text to Date.<br>
**Reason:** Ensures proper sorting, filtering, and time-based analysis.<br>

3. Applied Currency Format<br>
**Action:** Formatted the Total Revenue column into a Currency format.<br>
**Reason:** To maintain consistency in financial data presentation and improve readability during analysis.<br>

4. Checked for Duplicates< br>

  **Action:** Verified all records for duplicate values.<br>
  **Result:** No duplicates were found in the dataset.<br>
  **Reason:** Ensures data integrity and prevents double counting in analysis.<br>

5. Validated Total Amount Calculation <br>

  **Action:** Cross-checked that Total Amount = Price × Quantity for all records.<br>
  **Result:** All calculations were accurate with no discrepancies.<br>
  **Reason:** To ensure accuracy of revenue reporting and confirm data reliability.<br>

## WireFrame
![Metrogoods overview](https://github.com/user-attachments/assets/b2c18c9d-fe30-4162-8295-447b318eef0c)

![Metrogoods customer details](https://github.com/user-attachments/assets/a4badf26-c85d-4154-b498-e082dead8f54)


## Concepts Adopted in the Dashboard Design
To build the MetroGoods Sales Analysis dashboards, several Power BI concepts and techniques were applied to ensure the dashboards were both interactive and insightful:
Power Query for Data Preparation


### Power Query was used to clean, transform, and shape the dataset before loading it into the data model.


 *Tasks included removing duplicates, handling missing values, standardizing data types, and creating calculated columns to support analysis.


* This ensured the dataset was reliable and ready for advanced analysis.


### Parameters for KPI Flexibility


* Parameters were created to streamline the use of various KPIs such as Total Sales, Transactions, Quantities, Number of Customers, and Average Price.


 This allowed users to dynamically switch between KPIs and analyze performance without needing multiple static visuals.


### Bookmarks for Navigation & Filter Reset


* They were also applied to reset filters/selections back to default, improving user experience and reducing the need for manual slicer adjustments.


### Drill Through and Drilldown


* Drilldown enabled users to move from high-level summaries (e.g., sales by category) to more detailed breakdowns (e.g., by month or customer segment).


* Drill through allowed focused analysis on specific customers or product categories, enabling transaction-level exploration.

### DAX for Custom KPIs and Indicators


* DAX (Data Analysis Expressions) was used extensively to create calculated measures such as Sales Growth vs Previous Month, Average Price Direction, and Transaction Counts.


* Directional indicators (↑/↓) were added to quickly show whether performance metrics improved or declined, enhancing clarity for business users.


## Key insights
![MetroGoods Stores Sales Analysis transaction_page-0001](https://github.com/user-attachments/assets/3ffe36ae-ea5a-4fe5-b5e0-7fd81e8995dd)

Key Insights from Metro Goods Dataset

1. **Overall Business Performance**

* The store generated $456,000 in total sales from 1,000 transactions and 1,000 unique customers.

* A total of 2,514 items were sold, with an average selling price of $179.89 per unit.
* Each customer made only one purchase, highlighting that all customers are one-time buyers.

2. **Category Performance**

* Clothing attracted the highest number of customers (351) and sold the most quantity (894 units).

* Beauty products recorded the least customers (307) and generated the lowest revenue, although it had the highest average price.

* Electronics was the top revenue-generating category, showing higher value per purchase.

3. **Gender Insights**

* Purchases were fairly balanced across genders, with female customers leading slightly at 51% compared to 49% for males.

* Females dominated Beauty purchases, while males led in Electronics and Clothing categories.

4. **Demographics**

* Middle-aged adults (36–55 years) were the most active buyers, contributing the highest number of transactions.

* Teenagers recorded the lowest participation, showing limited engagement with the store’s offerings.

5. **Seasonality & Trends**

* May was the peak month for sales, while September marked the lowest-performing period.

* Most products sold and revenue generated fell within the low-price range of $0–50, whereas the $51–300 price range accounted for the least activity.


  ## Recommendations for Metro Goods Stores


### Category Strategy

* Since Electronics drives the most revenue, maintain strong promotions but also introduce value-added services (e.g., warranties, installation support).

* For Clothing (highest customer count & quantity sold), run seasonal collections and bundle deals to boost frequency.

* For Beauty products (low revenue but high average price), consider affordable variants, promotional kits, or influencer marketing to drive volume.

### Gender-Focused Campaigns

* Expand female-focused marketing for Beauty products (social media campaigns, beauty influencer partnerships).

* Strengthen male-targeted promotions for Clothing and Electronics (sports-related, gadget launches, bundles).

### Demographic Targeting

* Double down on middle-aged adults (36–55) with family and lifestyle bundles, since they drive the most transactions.

* Engage teenagers and young adults through trend-driven, budget-friendly products and social media campaigns (TikTok/Instagram).

### Seasonality & Pricing

* Capitalize on May’s peak sales period with planned major sales events (e.g., “Metro Mega Sale Month”).

* Address September’s low sales with back-to-school discounts, festival promotions, or clearance events.

* Since most purchases happen at the $0–50 range, diversify product pricing tiers to capture mid-range customers ($51–300).

### Customer Experience

* Collect customer feedback at checkout to understand why they don’t return.

* Improve after-sales engagement (thank-you emails, product usage tips, personalized reminders).

* Strengthen delivery and in-store experience to enhance satisfaction.






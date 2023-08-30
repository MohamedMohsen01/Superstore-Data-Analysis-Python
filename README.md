# Superstore Sales Analysis Project

#### By: [Mohamed Mohsen](https://www.linkedin.com/in/mohamedmohsen01/)



# Executive Summary

In this project I have performed an exploratory data analysis (EDA), on sales data obtained from the Super Store. The main objective of this analysis is to gather insights about aspects of the business such as customer behavior, product categories, sales patterns and geographical trends. By investigating thought provoking questions I have uncovered information that can greatly assist in making informed decisions and developing effective strategies, for the Super Store.



# Data Description

This table contains 21 columns and 9993 rows.

**Data Dictionary**

| Column                  | Description                                  | Data Type      |
| :---------------------- | :--------------------------------------------| :------------- |
| Row ID                  | Unique ID for each row.                      | int            |
| Order ID                | Unique Order ID for each Customer.           | object         |
| Order Date              | Order Date of the product.                   | datetime       |
| Ship Date               | Shipping Date of the Product.                | datetime       |
| Ship Mode               | Shipping Mode specified by the Customer.     | object         |
| Customer ID             | Unique ID to identify each Customer.         | object         |
| Customer Name           | Name of the Customer.                        | object         |
| Segment                 | The segment where the Customer belongs.      | object         |
| Country                 | Country of residence of the Customer.        | object         |
| City                    | City of residence of of the Customer.        | object         |
| State                   | State of residence of the Customer.          | object         |
| Postal Code             | Postal Code of every Customer.               | int            |
| Region                  | Region where the Customer belong.            | object         |
| Product ID              | Unique ID of the Product.                    | object         |
| Category                | Category of the product ordered.             | object         |
| Sub-Category            |Sub-Category of the product ordered.          | object         |
| Product Name            | Name of the Product                          | object         |
| Sales                   | Sales of the Product.                        | float          |
| Quantity                | Quantity of the Product.                     | int            |
| Discount                |Discount provided.                            | float          |
| Profit                  | Profit/Loss incurred.                        | float          |







# Methodology

**1. Data Collection**

 - Collected the dataset from Kaggle website >> Link to the data source: (https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)


**2. Data Understanding**

- Conducted an in-depth exploration of the dataset's structure, comprehensively documenting available columns, data types, and referring to the data dictionary for clarification.
- Gained an understanding of the specific business questions or objectives that need to be addressed using the dataset.


**3. Data Pre-processing and Cleaning:**

Enhanced the dataset's quality by applying data cleaning methods. I adjusted data formats and structures to ready the dataset for analysis.

- Used approaches like filling in missing data, based on the kind of missing data.
- Checked for duplicate records to maintain accurate and reliable data.
- Converted the data type of specific columns to approporaite data type for better optimization.


**4. Feature Engineering**

Created new variables from existing data that provided additional insights, such as:

- Generated a column named  `month_year`  to extract the month and year of the `Order Date` column in each transaction. This additional data will be invaluable for discerning sales trends on a monthly basis for each year.

- Generated another new column titled `Profit Margin` calculated by dividing the overall profit by the total sales. This metric provides insight into the profitability ratio.

**5. Exploratory Data Analysis (EDA):**

The process of exploratory data analysis is done by answering the listed questions and objectives outlined within this project's scope.





## Functions and methods used:

- head()
- tail()
- describe()
- info()
- shape
- isna().sum()
- fillna()
- duplicated().sum()
- pd.to_datetime()
- describe().transpose()
- nunique()
- unique()
- sort_values()
- value_counts()
- reset_index()
- plt.figure()
- plt.pie()
- plt.title
- sum()
- groupby()
- plt.xlabel()
- plt.ylabel()
- rename()
- plot(kind='bar')
- plt.xticks()
- plt.barh()
- mean()
- dt.year
- dt.month
- plt.grid(True)
- pd.Grouper()
- plt.lineplot
- agg()
- size()
- plt.subplots()
- set_xlabel()
- set_ylabel()
- set_title()
- tick_params()




# Business Questions I've answered

Enhanced the initial data exploration process during the EDA phase, gaining a profound understanding of the variables and their distributions. 
Some of the questions I've answered based on the data:


### Customer Analysis

1. What are the distinct customer segments?
2. How many customers are there in each segment?
3. Represent the distribution of customers using a pie chart.
4. What is the cumulative sales across different customer categories?
5. Visualize the segmentation of customers based on sales using a bar chart.
6. How many orders have been placed by each customer?
7. Which customers are repeat buyers and what are their order counts?
8. List the top 10 customers by total sales.

### Product and Product Category Analysis

1. Identify the various product categories.
2. How many sub-categories exist within each category?
3. Calculate the total sales for each product category.
4. Determine the frequency of each product category.
5. Assess the overall profit across different product categories.
6. Analyze the total sales across various sub-categories.
7. Examine the overall profit across different sub-categories.
8. Which products exhibit the highest sales performance at the Super Store?
9. Which products exhibit the highest profit performance at the Super Store?
10. Create a visualization showcasing the categories and sub-categories within California State.
11. Investigate regional discrepancies in average sales and profits for the "Canon imageCLASS 2200 Advanced Copier."
12. Investigate regional discrepancies in average sales and profits for the "Fellowes PB500 Electric Punch Plastic Comb Binding Machine with Manual Bind."
13. How does the application of discounts influence sales?
14. Explore the relationship between sales and discount ratios.
15. Analyze the correlation between profits and discounts.
16. Calculate the average profit margin percentage for each category.
17. Generate a bar chart utilizing a red color scheme to visualize profit margin percentages across categories.
18. Compare overall profit with profit margin percentages.

### Sales Trend Over Time

1. Determine the occurrence frequency for each year.
2. Illustrate the yearly sales trend using a line graph.
3. Display the yearly sales and profits trend on a single chart.
4. Display the quarterly sales and profits trend on a single chart.
5. Calculate the frequency of sales for each month.
6. Visualize the monthly sales trend.
7. Analyze the monthly variations in total sales and profit from 2014 to 2017 for the "Standard Class" segment.

### Geographical Analysis

1. Identify the city with the highest sales and profits.
2. Create a visual comparison of sales and profits across different cities.
3. Determine the region with the highest sales and profits.
4. Create a visual comparison of sales and profits across different regions.
5. Identify the state with the highest sales and profits.
6. Visualize the distribution of customer segments within each region.
7. Create a visual comparison of sales and profits across different states.
8. Enumerate the types of shipping modes.
9. Calculate the frequency of each shipping method.
10. Generate a pie chart for a visual representation of shipping mode distribution.
11. Analyze total sales for each shipping mode and customer segment.
12. Visualize total sales per customer segment and shipping mode using a bar chart.
13. Calculate the total profit per customer segment and shipping mode.
14. Visualize total profits per customer segment and shipping mode using a bar chart.
15. Determine the number of customers in each state.
16. Compute the average sales based on state and shipping mode.





# Overview of the Analysis Approach


**1. Understanding Customer Behavior:**

The analysis begins by looking closely at different types of customers and their distinctive characteristics. I've delved into how these customer groups are spread out and their contributions to our sales. By visualizing how sales are divided among these groups, we can figure out which customer segments are the main drivers of our revenue. Furthermore, I've pinpointed repeat customers, giving us insights into customer loyalty and engagement.

**2. Examining Products and Categories:**

This report takes a deep dive into our Super Store's range of products. It focuses on identifying various product categories and their sub-categories, while also assessing how well they perform in terms of sales and profitability. This analysis uncovers which products stand out in both sales and profitability. Additionally, I've studied how discounts affect our sales and delved into the connection between sales, profit margins, and discounts.

**3. Trends in Sales Over Time:**

I've dug into the data to uncover patterns in our sales over time, examining yearly, quarterly, and monthly trends. Our visual representations paint a clear picture of how sales ebb and flow throughout the year and each quarter, and how these trends align with our profit patterns. Furthermore, I've scrutinized variations in monthly sales to shed light on any underlying factors influencing the data. Moreover, I've carried out a detailed analysis specifically on the sales and profit changes within the "Standard Class" segment from 2014 to 2017.

**4. Understanding Geographic Patterns:**

Our study has looked into patterns to gain insights into how sales and profits are distributed across cities, regions, and states. I've highlighted the cities, regions, and states that excel in sales and profits by using visual aids to showcase regional differences. Additionally, I've evaluated how different shipping methods impact our sales and profits, aiming to provide valuable insights into customer preferences.

**Benefits of This Analysis:**

This comprehensive exploratory data analysis equips the Super Store with valuable insights extracted from the available data. By addressing pertinent questions, we've unearthed crucial details about customer behavior, product performance, sales trends, and geographical dynamics. These insights are pivotal in making informed decisions to enhance operational efficiency and formulate strategies that set the stage for sustainable growth and success in today's fiercely competitive retail landscape.





# Results and Insights

- The analysis identified four main customer groups: Home Office, Corporate, and Consumer. These groups represent the various types of customers the Super Store serves.

- Among these groups, the largest is Consumer with 5191 Customers, followed by Corporate with 3020 Customers, and then Home Office with 1783 Customers. Home Office has the fewest customers.

- Consumer leads in sales with a total of `$1.16 million`, followed by Corporate with $7 million, and Home Office with `$4.2 million`.

- Notably, repeat buyers exist in all segments, showing strong customer loyalty. Most repeat buyers are in the Consumer and Corporate segments, indicating effective customer engagement.

- The analysis also identified product categories: Furniture, Office Supplies, and Technology, each with sub-categories.

- Technology has the highest sales at `$836,154.03`, followed by Furniture with `$741,999.8`, and Office Supplies with `$719,047.03`.

- For profitability in categories, Technology is on top with `$145,454.94` profit, then Office Supplies with `$122,490.80`, and Furniture with `$18,451.27`.

- Top-selling products include "Office Chairs" and "Phones." Interestingly, the "Copiers" sub-category stands out in profitability.

- "Phones" sub-category leads in sales with $330,007.05, followed by "Chairs" with `$328,449.1`, and "Storage" with `$223,843.6`. "Fasteners" has the lowest sales at `$3,024.28`.

- For profitability in sub-categories, "Copiers" leads with `$55,617.82`, followed by "Phones" with `$44,515.7`, and "Accessories" with `$41,936.63`. "Tables" show a loss of `$-17,725.48`.

- Top-selling and profitable products are "Canon imageCLASS 2200 Advanced Copier" and "Fellowes PB500 Electric Punch Plastic Comb Binding Machine with Manual Bind."

- Generally, higher discounts mean lower sales. This follows retail practices where deeper discounts attract more customers but reduce overall revenue.

- Some specific discount ratios like 0.45, 0.60, and 0.70 result in low sales, suggesting customer resistance to these discounts.

- Sales vary from around `$5,000` to over `$1 million`, with discounts ranging from 0% to 80%.

- Furniture has the smallest profit margin at 3.88%, Office Supplies at 13.80%, and Technology at 15.61%.

- Sales fluctuate over months, with peak sales in November 2017 at `$118,447.83` and lowest in February 2014 at `$4,519.90`.

- New York City has the highest sales and profit, followed by Los Angeles and Seattle. San Diego has the lowest profit.

- The "West" region excels in both sales and profits, highlighting effective cost management despite high sales.

- California, New York, and Texas have high sales, but Texas struggles with negative profits despite revenue.

These findings give insights into customer behavior, product performance, regional sales, and profitability.






# Conclusion

our data analysis has given us some important findings about our customers, products, and regions. I've identified three main customer groups: Home Office, Corporate, and Consumer. Among these, the Consumer group is the biggest in terms of both customers and sales.

We've noticed that many customers like to buy from us again, especially in the Consumer and Corporate groups. This shows that our strategies for engaging with customers are working well.

When it comes to products, technology items are the most popular and profitable. Some products, like "Office Chairs" and "Phones," are really popular and make us a lot of money. And interestingly, "Copiers" are bringing in the most profit among all products.

We've also looked at how offering discounts affects our sales. Generally, bigger discounts mean we sell more, but we also make less money overall. Some discount levels, like 45%, 60%, and 70%, don't lead to much sales, which tells us our customers might not like those discounts.

Different parts of the country have different sales and profits. New York City is our best place for both sales and profits. And the western part of the country does really well too, making us a lot of money.

In simple words, some states like California and New York are really good for us, making us a lot of money. But in places like Texas, even though we sell a lot, we're not making much profit. This shows there's room to improve how we manage costs in those areas.

All in all, this analysis gives us smart ideas to keep our customers happy, manage discounts better, and make the most of different parts of the country. This will help us do even better in the competitive world of retail.





# Recommendations

- People who've shopped with us before tend to come back. Let's make them feel special with personalized offers and loyalty perks.

- Tech stuff sells well and makes good money. We should focus more on these items and maybe offer related products to boost sales.

- While discounts attract customers, really big discounts can hurt overall profits. Let's find the right balance and avoid certain percentages that don't work so well.

- Some places do great, like the "West" region. We can share their tactics with others to help them improve.

- Certain states like California and New York sell a lot, while Texas sells a lot but doesn't make much profit. We need to figure out why and fix it.

- Sales change throughout the year. We should plan our promotions and products based on when people shop the most.

- Some products make more money than others. We need to focus on these winners and maybe let go of products that don't make us much.

- To make more money in regions with low profits, we need to find ways to spend less while keeping customers happy.

- Always look for ways to attract better customers and offer them more. This will help us make more money and stand out in the market.

By following these suggestions, we can make customers happier, sell more of the right stuff, and make smarter decisions in different parts of the country. This will help us do even better in the retail world.

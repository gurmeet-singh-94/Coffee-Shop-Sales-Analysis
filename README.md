## Coffee Shop Sales Analysis | MS-Excel
### The objective of this project is to analyze the sales data to have useful insights which will help the enhance the performance of the Coffee Shop.
#### -------------------------------------------------------------------------------------------------------------------------------------------------------------
### -->> Data Loading , Processing and Cleaning.
#### Upload Excel File into Power Query Editor 
#### Data -> Get Data -> From File -> Choose From Excel Workbook -> Transform Data

##### 1. Detect data type of each column. 
##### 2. Added new conditional column named it (Size) in which we replace values Lg into Large, Rg into Regular and Sm into Small and the rest of them is Not Defined.
##### 3. Make a Custom Column named Total Bill, in which we multiply unit price and transaction_qty and change the data type of Total Bill into Currency.
##### 4. Extract time from transaction_time column and change their data type to time.
##### 5. Make new columns - Day Name, Hour, Day of Week, Month and Month Name from Transaction Date Columns.

##### Then go to (Close and Load to) option and select add to data model option then ok.
### -->> Pivot Tables, Charts And Graphs.
#### Mentioned below are the Pivot Tables , Charts and Graphs through which we create Dashboard :--
##### 1. Sum of Transactions by Hour -- Put Hour column in Rows and transaction_qty column in values having aggregate function of sum . Make Line Chart from this Pivot Table which will help in analyzing the sum of transactions in each hour.
##### 2. Sum of Products by Category -- Put product_category column in rows and Total_Bill column in values having aggregate function of sum. Make Pie Chart from this Pivot Table which wiil help in analyzing the contribution of each product type Category in sales.
##### 3. Sum of Transactions by Order Size -- Put Size column in rows and Transaction_id column in values having aggregate function of count. Make Pie Chart from this Pivot Table which wiil help in analyzing the contribution of each product based on their size.
##### 4. TOP FIVE PRODUCT TYPE --  Put product_type column in rows and Total_Bill column in values having aggregate function of sum. Make Clusterd Bar Chart which shows the top five products in sequence.
##### 5. Count of Transactions Day Wise -- Put Day Name column in rows and Total_Bill column in values having aggregate function of count. Make Clustured Columns which which shows no. of transactions day wise.
##### 6. Count of Transactions by Store Location -- Put Store_Location column in rows and Total_Bill column in values having aggregate function of sum. Make Clustured Columns which which shows no. of transactions store location wise. 
##### 7. Add Two Slicers -- Month Name, Day Name which helps in filtering the data.
### -->>> Make four Cards -- Total Sales, Total Transactions, Average Bill per Person, Average Order
![Screenshot 2025-03-24 114234](https://github.com/user-attachments/assets/364ffb3f-25fb-4583-a4a6-81d9c14b8ebb)
### -->> INSIGHTS
#### . Peak sales occur between 7 AM and 9 AM, confirming that morning hours are the busiest.
#### . Sales drop after 10 AM and remain steady throughout the day.
#### . Barista Espresso is the highest-selling item.
#### . Coffee products dominate (39%), followed by Bakery items (28%).Tea contributes 6%, indicating potential for expansion.
#### . 31% of orders are Regular-sized.30% are Large, while another 30% are Undefined. Only 9% of orders are Small.
#### . Thursday ($21,654.00) and Friday ($21,701.00) see the highest transactions.Saturday has the lowest transaction volume ($20,510.00).
#### . Hell’s Kitchen ($50,735.00) and Astoria ($50,599.00) are the highest-performing locations.Lower Manhattan ($47,782.00) lags behind.
### -->> RECOMMENDATIONS
#### . Enhance marketing for off-peak hours (post-10 AM) to maintain steady sales
#### . Promote weekend discounts or special offers to drive Saturday sales.
#### . Encourage upselling by offering combo deals for small orders.
#### . Introduce afternoon promotions and rewards to increase midday and evening sales.
#### . Optimize pricing or introduce special deals for Lower Manhattan to improve performance
#### . Introduce Happy Hour Discounts (Offer buy-one-get-one (BOGO) deals or discounts on select drinks during low-sales periods (10 AM - 4 PM).
#### . Weekend Brunch Combos – Offer a breakfast meal deal (coffee + pastry or sandwich) at a bundled price.
#### . Launch Midday Special Combos – Pair coffee with a snack (e.g., coffee + muffin) at a discounted price.
#### . Promote Afternoon Beverages – Market non-caffeine drinks (e.g., smoothies, flavored teas, cold brews) to attract different customers.





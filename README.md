# Retail Analytics-Project-PowerBI-Data-Visualization

# OVERVIEW
Retail businesses, from supermarkets to convenience stores, are constantly seeking ways to better understand their customers and improve their operations.This project is aimed at gaining insights and analyzing trends and patterns on the retail data.The analysis has been divided into three sections-Revenue Analysis,Sales Analysis and Customer Analysis. Power BI , a powerful data visualisation tool was used to gain meaningful insights on this retail data.

# ABOUT THE DATA
The dataset was obtained from Kaggle:https://www.kaggle.com/datasets/prasad22/retail-transactions-dataset.
It is a comprehensive dataset comprising of nearly 10 lakhs transaction made by many customers on different products in different stores present in various regions of US.

**Columns in Dataset**
1. **Transaction_ID:** A unique identifier for each transaction, represented as a 10-digit number. This column is used to uniquely identify each purchase.
2. **Date:** The date and time when the transaction occurred. It records the timestamp of each purchase.
3. **Customer_Name:** The name of the customer who made the purchase. It provides information about the customer's identity.
4.**Product:** A list of products purchased in the transaction. It includes the names of the products bought.
5. **Total_Items:**The total number of items purchased in the transaction. It represents the quantity of products bought.
6. **Total_Cost:** The total cost of the purchase, in currency. It represents the financial value of the transaction.
7. **Payment_Method:** The method used for payment in the transaction, such as credit card, debit card, cash, or mobile payment.
8. **City:** The city where the purchase took place. It indicates the location of the transaction.
9. **Store_Type:** The type of store where the purchase was made, such as a supermarket, convenience store, department store, etc.
10. **Discount_Applied:** A binary indicator (True/False) representing whether a discount was applied to the transaction.
11. **Customer_Category:** A category representing the customer's background or age group.
12. **Season:** The season in which the purchase occurred, such as spring, summer, fall, or winter.
13. **Promotion:** The type of promotion applied to the transaction, such as "None," "BOGO (Buy One Get One)," or "Discount on Selected Items."

# APPROACH USED:
Data is loaded into Power Query and the following transformations were done:
Using tools like Column Quality,Column profile and Column distribution- each attribute of a dataset is studied for the presence of error,valid values,empty values,distribution of data,identification of unique values,etc..

# Feature Engineering:
1. ** New column "Year" was created from date column
2. **New column "MonthName" was created from date column
3. **New column "Quarter" was created from date column
4. ** New column "week of year" was created from date column
5. ** Created a conditional column namely Holiday or working day using conditional statements

# DAX Measures:
Measure table was created in PowerBI front end to store all measures.
Total Revenue,Total customers,Total transactions,Total customers who opted for BOGO(Buy one Get one option) were created using various DAX functions

# LAYOUTS:
# REVENUE ANALYSIS:
1. ** Used cards to showcase TotalRevenue,Total Quantity Sold,Total transactions.
2. ** Used Bar chart to show the revenue trend on month to month basis.
3. ** Used Area chart to study the pattern of revenue obtained by each store
4. ** Used Piechart to study the total proportion of revenue obtained by season
5. ** Donut chart was used to revenue obtained by daytype(Holiday or working day)
6. ** Slicers are created for year,quarter and week of year to show interactivity on data and to gain more insights.

# SALES ANALYSIS:
1. ** Stacked bar chart was used to study on the pattern of sales done on each store type and on day type
2. **Area chart was used to study the sales carried on different cities
3. **Used Piechart to study the total proportion of sales obtained by various customers
4. **Donut chart was used to sales obtained by month
5. **Slicers were created for each store type to get more insights on sales by each store

# CUSTOMER ANALYSIS:
1. **A map visual was created to study the total customers from different cities
2. **A Area chart was created to study the trend of customer purchasing by year
3. **A card was created to show the no.of customers who purchased products that are in promotion type
4. **A matrix visual was used to study the customer preferences on Promotion
5. **Bar chart was created to study the customer behavior on payment methods
6. **A treemap was created to study the customer behavior on preferred day to buy products.

Additionally buttons were created on each analysis dashboard page to quickly navigate to other page for better insights and deeper understanding.

# CONCLUSION
1. **Overall,storetypes such as Pharmacy,Supermarket,Warehouse club had good sales and higher revenue.
2. **Revenue obtained was much higher on working days than holidays and there is influence of season on revenue.
3. **Highest number of items were sold in Boston followed by Dallas. Sales needs to be promoted in areas like Miami,San Fransciso and Atlantia.Promotions are a good way to draw customers to stores and this data explicity shows it.
4. **Promotion type such as BOGO were opted by 170K people.Customers prefer promotions such as BOGO, discounts on a larger basis.

Thus through this study, we have identified areas/stores that needs much concentration for promotion of sales and products which can be obtained via various promotion methods such as one-day free sample option,BOGO,discounts,etc.. and much more insights.

# PLSQL-WINDOW-FUNCTION-Byusa-Arsene
PLSQL-Assignment
# **Buisiness Scenario**
## *Buisiness context*
### Company type:
- service_based company
### Department
- Analytics Department
### Industrty
- Delivery services industry

## *Data challenges*
The A&B_shopping&delivery_services has had a big problem finding a way to manage customers data and reduce duplication and ensure accurate deliveries. They had a problem in recording inventories which led to overselling and miscategorization. Transaction has been an issue that needs a solution as well, since the buisiness do not have a way to to link customers with products a payment, this lead to financial discrepancies and delivery erros.

## *Expected outcome*
- The development of the database will help the buisiness to reduce data duplication and ensure accurate deliveries of products to the right customer.
- Every sales will be monitored making it easy to know who brought which kind of product or who purchased this product and know where to deliver the product. Thus ensuring a smooth tracking of payment and delivery orders.
- The database will help in keeping record of the products in stock those reducing the risk of selling out for the buisiness and also helping the customers to know which kind of products are in stock and which one to purchase if needed.
- The most important outcome we expect is a a smooth running of operation for the buisiness and therefore ensuring customer satisfaction and ensuring that all data are well arranged to avoid mix-ups of data.

# **Success Criteria for A&B_Shopping**
- *Top 5 products per region/quarter → RANK()*: identifies the best selling product per region and rank them based on which region and product sold more.
- *Running monthly sales totals → SUM() OVER()*: adds up total sales that was recieved monthly, therefore being able to track revenue generated
- *Month-over-month growth → LAG()/LEAD()*: compares this month total sales to the month before thus being able to track an increase or decrease in revenue.
- *Customer quartiles → NTILE(4)*: divide customers into different groups based on how much they spend thus being able to reward the customer who spends more.
- *3-month moving averages → AVG() OVER()*: calculate the average number of orders over 3months thus being able to predic orders and maintain invetories.


# **References**
- https://www.sqltutorial.org/sql-window-functions/
- https://www.geeksforgeeks.org/sql/window-functions-in-sql/
- https://www.youtube.com/watch?v=a9u2yZvsqHA
- https://stackoverflow.com/questions/65311362/how-to-deal-with-sql-database-in-github
- https://www.sqlservertutorial.net/sql-server-window-functions/sql-server-ntile-function/
- https://www.sqltutorial.org/sql-window-functions/sql-cume_dist/
- https://www.sqltutorial.org/sql-window-functions/sql-lag/
- https://www.sqltutorial.org/sql-window-functions/sql-lead/
- https://www.youtube.com/watch?v=a9u2yZvsqHA
- https://www.youtube.com/watch?v=cE3sCuL4L6c&list=PLX6xdk86h_0xpW82Q0YkdN6xpHa6hvHjO&index=6


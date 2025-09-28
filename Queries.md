# ** Window Function Implementation**
## ** Ranking**
### *Row_Number()*
This query calculates the total revenue per customer by joining the customers table and the transaction tables. This query groups the data by Customer_id and customer_name to aggregate the amount from transaction. Row_number() assigns a unique sequential number to each customer based on there total revenue in descending order, helping identify the top customers with a high spending, thus offering them special offers.


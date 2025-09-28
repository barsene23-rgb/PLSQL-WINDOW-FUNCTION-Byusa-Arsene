# **Window Function Implementation**
## **Ranking**
### *Row_Number()*
This query calculates the total revenue per customer by joining the customers table and the transaction tables. This query groups the data by Customer_id and customer_name to aggregate the amount from transaction. Row_number() assigns a unique sequential number to each customer based on there total revenue in descending order, helping identify the top customers with a high spending, thus offering them special offers.
 
 ***query***

SELECT C.customer_ID,C.customer_NAME,
sum(T.Amount) AS Total_Revenue,
row_number() over(order by sum(T.Amount) desc) AS Row_Num
FROM Customers C
join Transaction T ON C.Customer_id = T.Customer_id
group by C.customer_id, C.Customer_name
order by Total_Revenue desc;

***output***

![Queries](row_num.png)

### *Rank()*
This query calculates the total revenue per customer by joining the customers table and the transaction table. This query groups the data by customer_id and customer_name then aggregate the amount from transactions. Rank() assigns a rank to each customer based on total revenue in descending order, with ties receiving the same rank. The result helps identify top customers that spend a lot and therefore being able to provide special offers.


***query***

SELECT C.customer_id,C.customer_name,
sum(T.amount) as Total_revenue,
rank() over (order by sum(T.amount) desc)as rank_value
FROM customers C 
join transaction T on C.customer_id = T.customer_id
group by C.customer_id, C.customer_name
order by total_revenue desc;

***output***



## Validate using queries against Redshift Table

Here are the queries against Redshift Table to confirm whether data is copied or not successfully.

```sql
SELECT * FROM orders LIMIT 10

SELECT count(1) FROM orders

SELECT count(*) FROM orders

SELECT order_status, count(*) AS order_count
FROM orders
GROUP BY order_status


```

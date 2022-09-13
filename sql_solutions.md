# SQL_Solutions

## Index
1. [2602 Basic Select](#2602-Basic-Select)
2. [2603 Customer Address](#2603-Customer-Address)
3. [2604 Under 10 or Greater Than 100](#2604-Under-10-or-Greater-Than-100)
4. [2605	Executive Representatives](2605-Executive-Representatives)
5. 







## 2602 Basic Select

Your company is doing a survey of how many customers are registered in the states, however, lacked to raise the data of the state of the 'Rio Grande do Sul'.

Then, you must show the names of all customers whose state is 'RS'.
```sql
SELECT name FROM customers
WHERE state = 'RS'
```

## 2603 Customer Address
The company will make an event celebrating the 20th anniversary of the market, and for that we will make a great celebration in the city of Porto Alegre. We also invite all our customers who are enrolled in this city.

Your job is in having the names and addresses of customers who live in 'Porto Alegre', to deliver the invitations personally.
```sql
SELECT name, street FROM customers
WHERE city = 'Porto Alegre'
```
## 2604	Under 10 or Greater Than 100
The financial sector of the company needs a report that shows the ID and the name of the products whose price is less than 10 or greater than 100.

```sql
SELECT id, name FROM products
WHERE price<10 OR price>100
```

## 2605	Executive Representatives
The financial sector needs a report on the providers of the products we sell. The reports include all categories, but for some reason, providers of products whose category is the executive, are not in the report.

Your job is to return the names of the products and providers whose category ID is 6.

```sql
SELECT products.name, providers.name FROM products
JOIN providers ON providers.id = id_providers
WHERE id_categories = 6
```

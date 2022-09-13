# SQL_Solutions

## Index
1. [2602 Basic Select](#2602-Basic-Select)
2. [2603 Customer Address](2603-Customer-Address)







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

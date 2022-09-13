# SQL_Solutions

## Index
1. [2602 Basic Select](#2602-Basic-Select)
2. [2603 Customer Address](#2603-Customer-Address)
3. [2604 Under 10 or Greater Than 100](#2604-Under-10-or-Greater-Than-100)
4. [2605 Executive Representatives](#2605-Executive-Representatives)
5. [2606 Categories](#2606-Categories)
6. [2607 Providers' City in Alphabetical Order](#2607-Providers'-City-in-Alphabetical-Order)
7. [2608 Higher and Lower Price](#2608-Higher-and-Lower-Price)
8. [2609 Products by Categories](#2609-Products-by-Categories)
9. [2610 Average Value of Products](#2610-Average-Value-of-Products)
10. [2611	Action Movies](#2611-Action-Movies)
11. [2613 Cheap Movies](#2613-Cheap-Movies)
12. [2614	September Rentals](#2614-September-Rentals)
13. [2615 Expanding the Business](#2615-Expanding-the-Business)
14. [2616	No Rental](#2616-No-Rental)
15. [2617	Provider Ajax SA](#2617-Provider-Ajax-SA)
16. [2618	Imported Products](#2618-Imported-Products)
17. [2619	Super Luxury](#2619-Super-Luxury)
18. [2620	Orders in First Half](#2620-Orders-in-First-Half)
19. [2621	Amounts Between 10 and 20](#2621-Amounts-Between-10-and-20)
20. [2622 Legal Person](#2622-Legal-Person)
21. [2623 Categories with Various Products](#2623-Categories-with-Various-Products)
22. [2624 Number of Cities per Customers](#2624-Number-of-Cities-per-Customers)
23. [2738 Contest](#2738-Contest)



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
## 2606 Categories
## 2607 Providers' City in Alphabetical Order

## 2608 Higher and Lower Price
## 2609 Products by Categories
## 2610 Average Value of Products
## 2611 Action Movies
## 2613 Cheap Movies
## 2614 September Rentals
## 2615 Expanding the Business
## 2616 No Rental
## 2617 Provider Ajax SA
## 2618 Imported Products
## 2619 Super Luxury
## 2620 Orders in First Half
## 2621 Amounts Between 10 and 20
## 2622 Legal Person
## 2623 Categories with Various Products
## 2624 Number of Cities per Customers
## 2738 Contest



# DVD Rental Database Analysis for SQL Project

In this project, we look into the DVD Rental Database and investigate a total of 10 queries in order to generate some insightful business conclusions.

![App Screenshot](https://www.google.com/imgres?imgurl=https%3A%2F%2Fdinosaurdracula.com%2Fwp-content%2Fuploads%2F2017%2F02%2F1-3.jpg&tbnid=o83eYLOa_84w-M&vet=12ahUKEwjE4rG23oOCAxV0VDUKHTXFDbEQMygBegQIARBS..i&imgrefurl=https%3A%2F%2Fdinosaurdracula.com%2Fblog%2Fold-video-store%2F&docid=RkqsCmgvXHvfFM&w=640&h=675&q=vintage%20dvd%20stores&ved=2ahUKEwjE4rG23oOCAxV0VDUKHTXFDbEQMygBegQIARBS)


The DVD rental database represents the business processes of a DVD rental store. The DVD rental database has many objects, including: 



## DVD Rental ER Model

![App Screenshot](https://www.postgresqltutorial.com/wp-content/uploads/2018/03/dvd-rental-sample-database-diagram.png)


## DVD rental database tables

There are 15 tables in the DVD Rental database:

- actor – stores actors data including first name and last name.
- film – stores film data such as title, release year, length, rating, etc.
- film_actor – stores the relationships between films and actors.
- category – stores film’s categories data.
- film_category- stores the relationships between films and categories.
- store – contains the store data including manager staff and address.
- inventory – stores inventory data.
- rental – stores rental data.
- payment – stores customer’s payments.
- staff – stores staff data.
- customer – stores customer data.
- address – stores address data for staff and customers
- city – stores city names.
- country – stores country names.
## To know about customers
Query 1: What countries are the customers coming from? 

Key feature to show is Distinct. Inner join will also be used to return Country.


```
SELECT DISTINCT(country) AS "Country", COUNT (country) AS "Customer Amount"  
FROM country
JOIN city on city.country_id=country.country_id
JOIN address on address.city_id=city.city_id
JOIN customer on customer.address_id=address.address_id
GROUP BY DISTINCT(country)
ORDER BY Country asc;
```

Query 2: What countries own the highest sales revenue?  

Key feature to show is Order by. 
Inner join will also be used to return Country and Sales Revenue.

```
SELECT DISTINCT(country) AS "Country", SUM (amount) AS "Sales Revenue"  
FROM country
JOIN city on city.country_id=country.country_id
JOIN address on address.city_id=city.city_id
JOIN customer on customer.address_id=address.address_id
JOIN payment on payment.customer_id=customer.customer_id
GROUP BY DISTINCT(country)
ORDER BY "Sales Revenue" desc
```

Query 3: What countries have the largest customer base? 

Key feature to show is Group by. Inner join will also be used to return Country and Customer Amount.

```
SELECT DISTINCT(country) AS "Country", COUNT (country) AS "Customer Amount"  
FROM country
JOIN city on city.country_id=country.country_id
JOIN address on address.city_id=city.city_id
JOIN customer on customer.address_id=address.address_id
GROUP BY DISTINCT(country)
ORDER BY "Customer Amount" desc;
```
From Query 1,2 and 3, knowing the origin of the customer base and its profits generating, staff could act on producing some cultural-related events to promote the stores since they have a clear picture of the target audience.

Query 4: Who are the top 10 customers per total sales? 

Key feature to show is AS. Group by and limit will be used in order to return Customer and Amount. 

```
SELECT first_name AS "First Name", last_name AS "Last Name", SUM(amount) AS "Amount"
FROM customer
JOIN payment on customer.customer_id=payment.customer_id
GROUP BY first_name, last_name
ORDER BY "Amount" desc
LIMIT 10
```
After getting the top 10 customers, rewards could be given and hence developing loyalty programs to retain customers.

## To know about films
Query 5: Who are the top 10 most popular actors on the rank? 

Key feature to show is Inner join. Order by will also be used to return Actors and Rental Rate.
```
SELECT first_name, last_name, (SUM (rental_rate)) AS "Rental Rate"
FROM actor a
JOIN film_actor fc ON a.actor_id=fc.actor_id
JOIN film ON fc.film_id=film.film_id
GROUP BY first_name, last_name
ORDER BY "Rental Rate" desc
Limit 10
```
From the above, some interesting facts are derived from the top 10. The rank could be utilised to draw potential customers' interests.  

Query 6: What are the top 10 films rented? 

Key feature to show is Limit. Order by will be also used to return Films and Rental Rate
```
SELECT title AS "Films"
FROM film
GROUP BY "Films"
ORDER BY SUM(rental_rate) desc
Limit 10
```
From the above, top 10 films that are highly popularized among customers are listed. Staff can hence suggest valid recommendations to customers. 

Query 7: What are the top 3 genres and what are their total sales?

Inner Join will be used. Group by and  in order to return Genres and Total Sales.
```
SELECT name AS "Genres", SUM (amount) AS "Total Sales"
FROM category
JOIN film_category ON category.category_id=film_category.category_id
JOIN film ON film_category.film_id=film.film_id
JOIN inventory ON film.film_id=inventory.film_id
JOIN rental ON inventory.inventory_id=rental.inventory_id
JOIN payment ON rental.customer_id=payment.customer_id
GROUP BY "Genres"
ORDER BY "Total Sales" desc
```
Through joining relevant tables and querying through the sum of the amount, the result shows that "Sports", 
"Animation" and "Action" are the most profit-earning films. 

Query 8: What is the average rental rate for each genre? 

Key feature is to show Average. Inner join and Group by will also be used to return Genre and Average Rental Rate.
```
SELECT name AS "Genres", AVG (rental_rate) AS "Average Rental Rate"
FROM category
JOIN film_category ON category.category_id=film_category.category_id
JOIN film ON film_category.film_id=film.film_id
GROUP BY "Genres"
ORDER BY "Average Rental Rate" desc
```
From the above, after calculating the average rate of rental, it is highlighted that "Games" has the highest average rental rate, in order words it is the most popular Genre among all.  

## To know about stores
Query 9: Which store is making more sales? 

Key feature to show is the Group by to return Store and amount.
```
SELECT store.store_id AS "Store", SUM (payment.amount)
FROM store
JOIN staff ON staff.store_id=store.store_id
JOIN payment ON staff.staff_id=payment.staff_id
GROUP BY "Store"
ORDER BY SUM (payment.amount) desc
```
Through Group by, joining the tables and summing up the payment amount, it is observed that store 2 has a higher sales amount, in order words having a better performance.

Query 10: Which store has higher free rental films rented?

Key feature is to show Count.
```
SELECT store.store_id AS "Store", COUNT (payment.amount=0)
FROM store
JOIN staff ON staff.store_id=store.store_id
FULL JOIN payment ON staff.staff_id=payment.staff_id
GROUP BY store.store_id
ORDER BY store.store_id desc
```
By joining the tables and counting the payment amount equal to 0, it is shown that store 2 has more films full-of-charge rented. 

## Download the PostgreSQL sample database

The above database can be downloaded via the link here: 

https://www.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip


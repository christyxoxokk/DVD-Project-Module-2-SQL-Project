# DVD-Project-Module-2-SQL-Project


# DVD Rental Database Analysis for SQL Project

In the project, we look into the DVD Rental Database and investigate the total of 10 queries in order to generate some insightful business conclusion.

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
Query 1: Where are the customers coming from? 

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

Query 6: What are the top 10 films rented? 

Key feature to show is limit. Order by will be also used to return Films and Rental Rate
```
SELECT title AS "Films"
FROM film
GROUP BY "Films"
ORDER BY SUM(rental_rate) desc
Limit 10
```


Query 7: What are the top 3 genres and what are their total sales?

Inner Join will be used. Group by and  in order to return Genres and Total Sales.


Query 8: What is the average rental rate for each genre? 

Key feature is to show Average. Inner join and Group by will also be used to return Genre and Average Rental Rate.


Query 9: Is a film with higher rating contribute to a higher rental rate?

Aggregate function average will be used to return 
## To know about stores
Query 8: Which store is making more sales? 

Key feature to show is the Group by to return Store and Sales.
## Download the PostgreSQL sample database

The above database could be downloaded via the link here: 

https://www.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip


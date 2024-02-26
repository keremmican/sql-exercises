### Question&Answer

1. Write an INNER JOIN query to see the city (city) and country (country) names together from the city table and the country table.
```js
SELECT city, country FROM city INNER JOIN country ON city.country_id = country.country_id
```
2. Write an INNER JOIN query to see the payment_id along with the first_name and last_name from the customer table and the payment table.
```js
SELECT payment_id, first_name, last_name FROM customer INNER JOIN payment ON customer.customer_id = payment.customer_id
```
3. Write an INNER JOIN query to see the rental_id along with the first_name and last_name from the customer table and the rental table.
```js
SELECT rental_id, first_name, last_name FROM customer INNER JOIN rental ON customer.customer_id = rental.customer_id
```

4. Write a LEFT JOIN query to see the city (city) and country (country) names together from the city table and the country table.
```js
SELECT city, country FROM city LEFT JOIN country ON city.country_id = country.country_id
```
5. Write a RIGHT JOIN query to see the payment_id along with the first_name and last_name from the customer table and the payment table.
```js
SELECT first_name, last_name FROM customer LEFT JOIN payment ON customer.customer_id = payment.customer_id
```
6. Write a FULL JOIN query to see the rental_id along with the first_name and last_name from the customer table and the rental table.
```js
SELECT first_name, last_name FROM customer FULL JOIN rental ON customer.customer_id = rental.customer_id
```
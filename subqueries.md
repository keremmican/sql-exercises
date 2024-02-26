### Question&Answer

1. In the film table, the film length is shown in the length column. How many films are there with a length greater than the average film length?
```js
SELECT * FROM film WHERE length > (
    SELECT AVG(length) FROM film
)
```
2. How many films in the film table have the highest rental_rate value?
```js
SELECT COUNT(*) FROM film WHERE rental_rate = (
    SELECT MAX(rental_rate) FROM film
)
```
3. List the films in the film table with the lowest rental_rate and replacement_cost values.
```js
SELECT * FROM film WHERE rental_rate = (SELECT MIN(rental_rate) FROM film)
AND replacement_cost = (SELECT MIN(replacement_cost) FROM film)
```
4. List the customers in the payment table who have made the most number of transactions.
```js
SELECT * FROM payment WHERE amount = (SELECT MAX(amount) FROM payment)
```
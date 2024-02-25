### Question&Answer

1. Show all the data in all columns of the "film" table where the replacement cost value is greater than or equal to 12.99 and less than 16.99 (using the BETWEEN - AND structure).
```js
SELECT * FROM film WHERE replacement_cost BETWEEN 12.99 AND 16.99
```
2. Show the data in the "first_name" and "last_name" columns of the ".actor" table where the "first_name" value is either 'Penelope', 'Nick', or 'Ed' (using the IN operator).
```js 
SELECT * FROM actor WHERE first_name IN ('Penelope', 'Nick', 'Ed')
```
3. Retrieve all the data in all columns of the "film" table where the "rental_rate" values are 0.99, 2.99, or 4.99, and the "replacement_cost" values are 12.99, 15.99, or 28.99 (using the IN operator).
```js
SELECT * FROM film WHERE rental_rate IN (0.99, 2.99, 4.99) AND replacement_cost IN (12.99, 15.99, 28.99)
```
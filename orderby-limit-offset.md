### Question&Answer

1. List the top 5 longest films (based on length) ending with the character 'n' in the film table.
```js
SELECT * FROM film WHERE title LIKE ('%n') ORDER BY length DESC LIMIT 5
```
2. List the next 5 shortest films (length ranging from 6 to 10) ending with the character 'n' in the film table.
```js
SELECT * FROM film WHERE title LIKE ('%n') ORDER BY length ASC OFFSET 5 LIMIT 5
```
3. Sort the first 4 entries in descending order based on the "last_name" column in the customer table, with the condition that the "store_id" is 1.
```js
SELECT * FROM customer WHERE store_id = 1 ORDER BY last_name DESC LIMIT 4
```
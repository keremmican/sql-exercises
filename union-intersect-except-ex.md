### Question&Answer

1. List all the data for the first_name column in the actor and customer tables.
```js
(SELECT first_name FROM actor)
UNION
(SELECT first_name FROM customer)
```
2. List the intersecting data for the first_name column in the actor and customer tables.
```js
(SELECT first_name FROM actor)
INTERSECT
(SELECT first_name FROM customer)
```
3. List the data for the first_name column that is present in the first table but not in the second table in the actor and customer tables.
```js
(SELECT first_name FROM actor)
EXCEPT
(SELECT first_name FROM customer)
```
4. Let's repeat the first 3 queries for duplicate data as well.
```js
(SELECT first_name FROM actor)
UNION ALL
(SELECT first_name FROM customer)
```
```js
(SELECT first_name FROM actor)
INTERSECT ALL
(SELECT first_name FROM customer)
```
```js
(SELECT first_name FROM actor)
EXCEPT ALL
(SELECT first_name FROM customer)
```
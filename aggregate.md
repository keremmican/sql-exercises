### Question&Answer

1. What is the average value of the rental rates in the "rental_rate" column of the film table?
```js
SELECT AVG(rental_rate) FROM film
```
2. How many films in the film table start with the character 'C'?
```js
SELECT COUNT(*) FROM film WHERE title LIKE ('C%')
```
3. What is the length (in minutes) of the longest film in the film table with a rental_rate value equal to 0.99?
```js
SELECT length FROM film WHERE rental_rate = 0.99 ORDER BY length DESC LIMIT 1
```
4. How many different replacement_cost values are there for films in the film table with a length greater than 150 minutes?
```js
SELECT COUNT(DISTINCT replacement_cost) FROM film WHERE length > 150
```
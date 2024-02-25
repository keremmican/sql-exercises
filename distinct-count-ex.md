### Question&Answer

1. Sort the distinct values from the "replacement_cost" column in the film table.
```js
SELECT DISTINCT replacement_cost FROM film
```
2. How many distinct values are there in the "replacement_cost" column in the film table?
```js
SELECT COUNT(DISTINCT replacement_cost) FROM film
```
3. How many film titles in the film table start with the character 'T' and have a rating equal to 'G'?
```js
SELECT COUNT(*) FROM film WHERE title LIKE ('T%') AND rating = 'G'
```
4. How many country names in the country table consist of 5 characters?
```js
SELECT COUNT(*) FROM country WHERE LENGTH(country) = 5
```
5. How many city names in the city table end with either the character 'R' or 'r'?
```js
SELECT COUNT(*) FROM city WHERE city ILIKE ('%r')
```
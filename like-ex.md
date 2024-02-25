### Question&Answer

1. Sort the country names in the "country" column of the country table that start with the character 'A' and end with the character 'a'.
```js
SELECT * FROM country WHERE country LIKE 'A%a'
```
2. Sort the country names in the "country" column of the country table that consist of at least 6 characters and end with the character 'n'.
```js
SELECT * FROM country WHERE country LIKE '______n'
```
3. List the film titles from the "title" column of the film table that contain the character 'T' regardless of case, with at least 4 occurrences of the character.
```js
SELECT * FROM film WHERE title ILIKE '%t%t%t%t%';
```
4. Retrieve data from all columns in the film table where the title starts with the character 'C', has a length greater than 90, and a rental_rate of 2.99.
```js
SELECT * FROM film WHERE title LIKE 'C%' AND length >90 AND rental_rate = 2.99;
```
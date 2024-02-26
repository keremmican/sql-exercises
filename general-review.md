### General Review

1. List the 4 longest films starting with the character 'K' in the film table with the lowest replacement_cost.
```js
SELECT * FROM film WHERE title LIKE ('K%') ORDER BY length DESC, replacement_cost ASC LIMIT 4
```
2. Which rating category contains the most number of films in the film table?
```js
SELECT * FROM film WHERE title LIKE ('K%') ORDER BY length DESC, replacement_cost ASC LIMIT 4
```
3. What is the name of the customer who has made the most number of purchases in the customer table?
```js
SELECT first_name FROM customer WHERE customer_id = (
    SELECT customer_id FROM payment GROUP BY customer_id ORDER BY SUM(AMOUNT) DESC LIMIT 1
)
```
4. List the category names and the number of films per category from the category table.
```js
SELECT category.name, COUNT(film_category.category_id) AS film_count
FROM category
LEFT JOIN film_category ON category.category_id = film_category.category_id
GROUP BY category.name
```
5. How many films in the film table have at least 4 occurrences of the character 'e' or 'E' in their names?
```js
SELECT COUNT(*)
FROM film
WHERE title ILIKE '%e%e%e%e%'
```

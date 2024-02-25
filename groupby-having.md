### Question&Answer

Group the films in the film table by their rating values.
```js
SELECT rating FROM film GROUP BY rating
```
When we group the films in the film table by the replacement_cost column, list the replacement_cost values for which the number of films is more than 50, along with the corresponding number of films.
```js
SELECT replacement_cost, COUNT(*) FROM film GROUP BY replacement_cost HAVING COUNT(*) > 50
```
What are the numbers of customers corresponding to each store_id value in the customer table?
```js
SELECT store_id, COUNT(*) FROM customer GROUP BY store_id
```
After grouping the city data in the city table by the country_id column, share the country_id information that contains the highest number of cities and the number of cities.
```js
SELECT country_id, COUNT(*) FROM city GROUP BY country_id ORDER BY COUNT(*) DESC LIMIT 1
```
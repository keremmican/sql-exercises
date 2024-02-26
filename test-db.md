### Question&Answer

1. Create a table in your test database called "employee" with column information: id (INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100).
```js
CREATE TABLE employee (
    id integer PRIMARY KEY,
    name varchar(50),
    birthday date,
    email varchar(100)
)
```
2. Let's add 50 pieces of data to the "employee" table using the 'Mockaroo' service.
   https://www.mockaroo.com
3. Let's perform 5 UPDATE operations to update other columns for each column.
```js
UPDATE employee
SET name = 'Kerem'
WHERE id = 1
```
4. Let's perform 5 DELETE operations to delete the respective rows for each column.
```js
DELETE FROM employee
WHERE id = 2
```


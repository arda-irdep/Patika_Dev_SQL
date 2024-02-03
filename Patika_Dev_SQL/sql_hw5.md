SELECT * from film
WHERE title LIKE '%n'
order by length DESC
LIMIT 5;

SELECT * from film
WHERE title LIKE '%n'
order by length
OFFSET 5
LIMIT 5;

SELECT * from customer
WHERE store_id = 1
ORDER by last_name DESC
LIMIT 4;
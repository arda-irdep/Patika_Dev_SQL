SELECT title, rating from film
group by title, rating;

SELECT replacement_cost, COUNT(*) FROM film
GROUP BY replacement_cost
HAVING COUNT(*) > 50;

SELECT COUNT(*) store_id from customer
GROUP by store_id;


SELECT country_id, COUNT(*) FROM city
GROUP BY country_id
ORDER BY COUNT(*) DESC;
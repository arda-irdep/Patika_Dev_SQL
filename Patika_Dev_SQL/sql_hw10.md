SELECT city, country from city
LEFT JOIN country ON country.country_id = city.city_id;

SELECT first_name, last_name from customer
RIGHT JOIN payment ON customer.customer_id = payment.customer_id;

SELECT first_name, last_name from customer
FULL JOIN rental ON customer.customer_id = rental.customer_id;


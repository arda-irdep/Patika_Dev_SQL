SELECT city, country from city
INNER JOIN country ON country.country_id = city.city_id;

SELECT first_name, last_name, payment_id from customer
INNER JOIN payment ON customer.customer_id = payment.customer_id;

SELECT first_name, last_name, rental_id from customer
INNER JOIN rental ON customer.customer_id = rental.customer_id;
	SELECT COUNT(*) FROM film
	WHERE length > (SELECT AVG(length) FROM film);

	SELECT COUNT(*) FROM film
	WHERE rental_rate = (SELECT MAX(rental_rate) from film);


	SELECT title FROM film
	WHERE rental_rate = (SELECT MIN(rental_rate) FROM film)
	AND replacement_cost = (SELECT MIN(replacement_cost) FROM film);


	SELECT first_name, last_name, COUNT(payment_id) FROM customer
	INNER JOIN payment ON customer.customer_id = payment.customer_id
	GROUP BY customer.customer_id, customer.first_name, customer.last_name
	ORDER BY total_purchases DESC;

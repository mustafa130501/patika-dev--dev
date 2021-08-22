SELECT COUNT(*) FROM film WHERE length > (SELECT AVG(length) from film)


 SELECT COUNT(*) FROM film WHERE rental_rate = (SELECT max(rental_rate) FROM film)



SELECT * FROM film WHERE rental_rate = (SELECT MIN(rental_rate) FROM film) AND replacement_cost = (SELECT MIN(replacement_cost) FROM film)




 SELECT * FROM customer WHERE customer_id IN (SELECT customer_id FROM payment WHERE amount = (SELECT max(amount) from payment))

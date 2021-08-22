SELECT city.city,country.country from  city LEFT JOIN country ON city.country_id= country.country_id


SELECT customer.first_name,customer.last_name,payment.payment_id from  payment RIGHT JOIN customer ON payment.customer_id=customer.customer_id



SELECT customer.first_name,customer.last_name,rental.rental_id from  rental FULL JOIN customer ON rental.customer_id=customer.customer_id

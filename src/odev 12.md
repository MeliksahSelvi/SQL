# SQL SORGULARIMIZ

### 1.film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?
```
SELECT COUNT(length) FROM film
WHERE length>
(
SELECT AVG(length) FROM film
);
```
### 2.film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?
```
SELECT COUNT(rental_rate) FROM film
WHERE rental_rate =
(
SELECT MAX(rental_rate) FROM film
);  
```
### 3.film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.
```
SELECT COUNT(rental_rate) FROM film
WHERE rental_rate =
(
SELECT MIN(rental_rate) FROM film
)
AND replacement_cost =
(
SELECT MIN(replacement_cost) FROM film
);
```
### 4.payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.
```
SELECT customer.customer_id,customer.first_name,customer.last_name,COUNT(payment.customer_id) FROM payment
INNER JOIN customer ON payment.customer_id=customer.customer_id
GROUP BY customer.customer_id,customer.first_name,customer.last_name
ORDER BY COUNT(payment.customer_id) DESC;
```

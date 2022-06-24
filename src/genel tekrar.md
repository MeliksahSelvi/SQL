# SQL SORGULARIMIZ

### 1.film tablosunda isminde en az 4 adet 'e' veya 'E' karakteri bulunan kaç tane film vardır?
```
SELECT COUNT(*) FROM film
WHERE title ILIKE '%E%E%E%E%';
```
### 2.film tablosundan 'K' karakteri ile başlayan en uzun ve replacenet_cost u en düşük 4 filmi sıralayınız.
```
SELECT title,length,replacement_cost FROM film
WHERE title LIKE 'K%'
ORDER BY length DESC,replacement_cost ASC
LIMIT 4;
```
### 3.film tablosunda içerisinden en fazla sayıda film bulunduran rating kategorisi hangisidir?
```
SELECT rating,COUNT(*) FROM film
GROUP BY rating
ORDER BY COUNT(*) DESC
LIMIT 1;
```
### 4.customer tablosunda en çok alışveriş yapan müşterinin adı nedir?
```
SELECT customer.first_name,customer.last_name, SUM(amount) FROM payment
INNER JOIN customer ON customer.customer_id=payment.customer_id
GROUP BY customer.customer_id
ORDER BY SUM(amount) DESC
LIMIT 1;
```
### 5.category tablosundan kategori isimlerini ve kategori başına düşen film sayılarını sıralayınız.
```
SELECT category.name, COUNT(*) FROM category
INNER JOIN film_category ON category.category_id=film_category.category_id
INNER JOIN film ON film_category.film_id=film.film_id
GROUP BY category.name;
```

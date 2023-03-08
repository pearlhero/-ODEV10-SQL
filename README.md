# -ODEV10-SQL
dvdrental sorgu senaryoları çözümleri
Sorgu 1- city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.
Çözüm 1- SELECT city, country FROM city
LEFT JOIN country 
ON city.country_id = country.country_id; 
<img width="478" alt="Ekran Resmi 2023-03-08 18 30 05" src="https://user-images.githubusercontent.com/116847744/223756335-e538ae05-2c4d-404f-acb2-0c384839cd0b.png">

Sorgu 2- customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.
Çözüm 2- SELECT first_name, last_name, payment_id FROM customer
RIGHT OUTER JOIN payment ON payment.customer_id = customer.customer_id;
<img width="687" alt="Ekran Resmi 2023-03-08 18 36 10" src="https://user-images.githubusercontent.com/116847744/223757851-2b037a07-0f21-4bb4-863a-ff8311a3b193.png">

Sorgu 3- customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.
Çözüm 3- SELECT first_name, last_name, rental_id FROM customer
FULL OUTER JOIN rental ON customer.customer_id = rental.customer_id;
<img width="645" alt="Ekran Resmi 2023-03-08 18 39 18" src="https://user-images.githubusercontent.com/116847744/223758481-c3dd5dd5-f50f-45f6-9feb-3151b2b01a49.png">

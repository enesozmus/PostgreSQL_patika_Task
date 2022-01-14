# PostgreSQL Task_9

<br>

## İstem → → city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
```sql
    SELECT city, country
    FROM city
    INNER JOIN country
    ON city.country_id = country.country_id;
```

<br>

## İstem → → customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
```sql
    SELECT payment.payment_id, customer.first_name, customer.last_name
    FROM customer
    INNER JOIN payment
    ON payment.customer_id = customer.customer_id;
    
```

<br>

## İstem → → customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
```sql
    SELECT rental.rental_id, customer.first_name, customer.last_name
    FROM customer
    INNER JOIN rental
    ON rental.customer_id = customer.customer_id;
```
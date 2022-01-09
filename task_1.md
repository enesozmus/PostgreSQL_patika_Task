# PostgreSQL Task_1 

<br>

## İstem → → film tablosunda bulunan title ve description sütunlarındaki bütün veriler.
```sql
    SELECT title, description FROM film;
```

<br>

## İstem → → film tablosunda bulunan film uzunluğu (length) 60'tan büyük VE 75'ten küçük olma koşullarını sağlayan bütün veriler.
```sql
    SELECT * FROM Film WHERE length > 60 AND length < 75;
```

<br>

## İstem → → film tablosunda bulunan rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koşullarını sağlayan bütün veriler.
```sql
    SELECT * FROM Film WHERE rental_rate = 0.99 AND (replacement_cost = 12.99 OR replacement_cost = 29.99);
```

<br>

## İstem → → customer tablosunda bulunan first_name sütunundaki değeri 'Mary' olan müşterinin last_name sütunundaki değeri nedir?
```sql
    SELECT last_name FROM customer WHERE first_name = 'Mary';
```

<br>

## İstem → → Film tablosundaki uzunluğu(length) 50'den büyük OLMAYIP aynı zamanda rental_rate değeri 2.99 ve 4.99 OLMAYAN bütün veriler.
```sql
    SELECT * FROM Film WHERE length < 50 AND ( rental_rate <> 2.99 AND rental_rate <> 4.99);
```
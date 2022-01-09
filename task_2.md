# PostgreSQL Task_2

<br>

## İstem → → film tablosunda bulunan replacement_cost değeri 12.99'dan büyük eşit ve 16.99'dan küçük olan bütün veriler. ( BETWEEN - AND yapısını kullanınız.)
```sql
    SELECT * FROM film WHERE replacement_cost BETWEEN 12.99 AND 16.99;
```

<br>

## İstem → → actor tablosunda bulunan first_name ve last_name sütunlardaki verileri first_name 'Penelope' veya 'Nick' veya 'Ed' değerleri olması koşuluyla sıralayınız. ( IN operatörünü kullanınız.)
```sql
    SELECT first_name, last_name FROM actor WHERE first_name IN ('Penelope', 'Nick', 'Ed');
```

<br>

## İstem → → film tablosunda bulunan rental_rate 0.99, 2.99, 4.99 VE replacement_cost 12.99, 15.99, 28.99 olma koşullarıyla sıralayınız. ( IN operatörünü kullanınız.)
```sql
    SELECT * FROM film WHERE (replacement_cost IN (12.99, 15.99, 28.99))  AND (rental_rate IN (0.99, 2.99, 4.99));
```
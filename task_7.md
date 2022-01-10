# PostgreSQL Task_7

<br>

## İstem → → film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.
```sql
   SELECT rating, count(title) FROM film GROUP BY rating;
```

<br>

## İstem → → film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.
```sql
   SELECT replacement_cost, COUNT(*) FROM film GROUP BY replacement_cost HAVING COUNT(*) > 50;
```

<br>

## İstem → → customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?
```sql
    SELECT store_id, COUNT(*) FROM customer GROUP BY store_id;
```

<br>

## İstem → → city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.
```sql
    SELECT country_id, COUNT(*) FROM city GROUP BY country_id ORDER BY COUNT(*) DESC LIMIT 1;
```
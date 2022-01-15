# PostgreSQL Task_12

<br>

## İstem → → film tablosundaki film uzunluğu → length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla -kaç tane- film vardır?
```sql
    SELECT COUNT(*)
    FROM film
    WHERE length > (SELECT AVG(length) FROM film);
```

<br>

## İstem → → film tablosunda en yüksek rental_rate değerine sahip -kaç tane- film vardır?
```sql
    SELECT COUNT(*)
    FROM film
    WHERE rental_rate = (SELECT MAX(rental_rate) FROM film);
```

<br>

## İstem → → film tablosunda en düşük rental_rate ve en düşük replacement_cost değerlerine sahip filmleri sıralayınız.
```sql
    SELECT *
    FROM film
    WHERE rental_rate = (SELECT MIN(rental_rate) FROM film) 
    AND replacement_cost = (SELECT MIN(replacement_cost) FROM film);
```
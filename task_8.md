# PostgreSQL Task_8

<br>

## İstem → → test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```sql
   CREATE TABLE employee (
        id SERIAL PRIMARY KEY,
        first_name VARCHAR(50) NOT NULL,
        last_name VARCHAR(50) NOT NULL,
        email VARCHAR(100) UNIQUE,
        birthday DATE
);
```

<br>

## İstem → → Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
```sql
    insert into employee (id, first_name, last_name, email, birthday) values (1, 'Catlaina', 'Wickham', 'cwickham0@comsenz.com', '2021-10-08');
    insert into employee (id, first_name, last_name, email, birthday) values (2, 'Richardo', 'Foldes', 'rfoldes1@odnoklassniki.ru', '2022-01-12');
    insert into employee (id, first_name, last_name, email, birthday) values (3, 'Tallia', 'Patterfield', 'tpatterfield2@va.gov', '2021-03-06');
    insert into employee (id, first_name, last_name, email, birthday) values (4, 'Hailey', 'Illwell', 'hillwell3@hhs.gov', '2022-01-12');
    insert into employee (id, first_name, last_name, email, birthday) values (5, 'Gael', 'Haymes', 'ghaymes4@wired.com', '2021-02-10');
    insert into employee (id, first_name, last_name, email, birthday) values (6, 'Waylan', 'Woodlands', 'wwoodlands5@goo.ne.jp', '2021-11-21');
    insert into employee (id, first_name, last_name, email, birthday) values (7, 'Linoel', 'Zoephel', 'lzoephel6@apache.org', '2021-11-28');
    insert into employee (id, first_name, last_name, email, birthday) values (8, 'Joscelin', 'Caudwell', 'jcaudwell7@cbslocal.com', '2021-03-01');
    insert into employee (id, first_name, last_name, email, birthday) values (9, 'Thatch', 'Plessing', 'tplessing8@nbcnews.com', '2021-10-06');
    insert into employee (id, first_name, last_name, email, birthday) values (10, 'Huberto', 'Brosio', 'hbrosio9@prlog.org', '2022-01-08');
    insert into employee (id, first_name, last_name, email, birthday) values (11, 'Noni', 'Goodredge', 'ngoodredgea@who.int', '2022-01-01');
    insert into employee (id, first_name, last_name, email, birthday) values (12, 'Thaddeus', 'Ogle', 'togleb@moonfruit.com', '2021-03-27');
    insert into employee (id, first_name, last_name, email, birthday) values (13, 'Humberto', 'Bernollet', 'hbernolletc@opera.com', '2021-09-23');
    insert into employee (id, first_name, last_name, email, birthday) values (14, 'Hendrick', 'Glass', 'hglassd@census.gov', '2021-08-14');
    insert into employee (id, first_name, last_name, email, birthday) values (15, 'Nataniel', 'Dorgon', 'ndorgone@indiatimes.com', '2021-06-11');
    insert into employee (id, first_name, last_name, email, birthday) values (16, 'Lindie', 'Lemoir', 'llemoirf@rakuten.co.jp', '2021-12-06');
    insert into employee (id, first_name, last_name, email, birthday) values (17, 'Lenora', 'Mousley', 'lmousleyg@businessweek.com', '2021-03-18');
    insert into employee (id, first_name, last_name, email, birthday) values (18, 'Kyle', 'Bridgewater', 'kbridgewaterh@geocities.jp', '2021-04-21');
    insert into employee (id, first_name, last_name, email, birthday) values (19, 'Leland', 'Flockhart', 'lflockharti@eventbrite.com', '2021-11-23');
    insert into employee (id, first_name, last_name, email, birthday) values (20, 'Dix', 'Mattaus', 'dmattausj@ft.com', '2021-08-11');
    insert into employee (id, first_name, last_name, email, birthday) values (21, 'Pepillo', 'Shattock', 'pshattockk@gov.uk', '2021-12-06');
    insert into employee (id, first_name, last_name, email, birthday) values (22, 'Gian', 'Woodyer', 'gwoodyerl@craigslist.org', '2021-10-02');
    insert into employee (id, first_name, last_name, email, birthday) values (23, 'Chico', 'Aronin', 'caroninm@jimdo.com', '2021-06-20');
    insert into employee (id, first_name, last_name, email, birthday) values (24, 'Benoite', 'Osichev', 'bosichevn@techcrunch.com', '2021-09-22');
    insert into employee (id, first_name, last_name, email, birthday) values (25, 'Gavan', 'Tingcomb', 'gtingcombo@wikimedia.org', '2021-07-14');
    insert into employee (id, first_name, last_name, email, birthday) values (26, 'Grace', 'Rendbaek', 'grendbaekp@tuttocitta.it', '2021-11-12');
    insert into employee (id, first_name, last_name, email, birthday) values (27, 'Mamie', 'Clarkin', 'mclarkinq@qq.com', '2021-01-22');
    insert into employee (id, first_name, last_name, email, birthday) values (28, 'Derrek', 'Barkas', 'dbarkasr@google.com.hk', '2021-10-18');
    insert into employee (id, first_name, last_name, email, birthday) values (29, 'Hewe', 'Uzelli', 'huzellis@latimes.com', '2021-08-01');
    insert into employee (id, first_name, last_name, email, birthday) values (30, 'Del', 'Binden', 'dbindent@ocn.ne.jp', '2021-02-21');
    insert into employee (id, first_name, last_name, email, birthday) values (31, 'Sabina', 'Dimmick', 'sdimmicku@dot.gov', '2021-02-10');
    insert into employee (id, first_name, last_name, email, birthday) values (32, 'Silvano', 'Olivetta', 'solivettav@exblog.jp', '2021-11-05');
    insert into employee (id, first_name, last_name, email, birthday) values (33, 'Maitilde', 'Sorbie', 'msorbiew@msu.edu', '2021-05-02');
    insert into employee (id, first_name, last_name, email, birthday) values (34, 'Etienne', 'Pizey', 'epizeyx@wired.com', '2021-09-06');
    insert into employee (id, first_name, last_name, email, birthday) values (35, 'Toddy', 'Luffman', 'tluffmany@1und1.de', '2021-10-04');
    insert into employee (id, first_name, last_name, email, birthday) values (36, 'Connie', 'Tobias', 'ctobiasz@amazon.de', '2021-09-06');
    insert into employee (id, first_name, last_name, email, birthday) values (37, 'Flo', 'Decourcy', 'fdecourcy10@cbslocal.com', '2021-10-06');
    insert into employee (id, first_name, last_name, email, birthday) values (38, 'Malcolm', 'Weagener', 'mweagener11@oakley.com', '2021-09-22');
    insert into employee (id, first_name, last_name, email, birthday) values (39, 'Mack', 'Stitle', 'mstitle12@stumbleupon.com', '2021-08-09');
    insert into employee (id, first_name, last_name, email, birthday) values (40, 'Raeann', 'Venus', 'rvenus13@networkadvertising.org', '2022-01-09');
    insert into employee (id, first_name, last_name, email, birthday) values (41, 'Mariele', 'Wrankmore', 'mwrankmore14@tripod.com', '2021-04-29');
    insert into employee (id, first_name, last_name, email, birthday) values (42, 'Jamil', 'Frederick', 'jfrederick15@i2i.jp', '2021-04-27');
    insert into employee (id, first_name, last_name, email, birthday) values (43, 'Gwen', 'Romao', 'gromao16@free.fr', '2021-04-21');
    insert into employee (id, first_name, last_name, email, birthday) values (44, 'Michale', 'Torrent', 'mtorrent17@jalbum.net', '2021-10-18');
    insert into employee (id, first_name, last_name, email, birthday) values (45, 'Lorrie', 'Fouracre', 'lfouracre18@tinyurl.com', '2021-08-03');
    insert into employee (id, first_name, last_name, email, birthday) values (46, 'Lutero', 'Nizet', 'lnizet19@g.co', '2021-05-27');
    insert into employee (id, first_name, last_name, email, birthday) values (47, 'Vannie', 'Basilotta', 'vbasilotta1a@uiuc.edu', '2021-07-29');
    insert into employee (id, first_name, last_name, email, birthday) values (48, 'Papageno', 'Haker', 'phaker1b@statcounter.com', '2021-08-12');
    insert into employee (id, first_name, last_name, email, birthday) values (49, 'Ronnica', 'Brann', 'rbrann1c@domainmarket.com', '2021-10-25');
    insert into employee (id, first_name, last_name, email, birthday) values (50, 'Stephanie', 'Clarson', 'sclarson1d@liveinternet.ru', '2021-12-09');
```

<br>

## İstem → → Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

### Id'si 1 ve adı Catlaina olan çalışanın email'i güncellendi
```sql
    UPDATE employee
    SET first_name = 'Catlaina', last_name = 'Wickham', email = 'demo_demo@test.com', birthday = '2021-10-08'
    WHERE id = 1;
```
### Id'si 2 ve adı Richardo olan çalışanın first_name'i Julia olarak güncellendi
```sql
    UPDATE employee
    SET first_name = 'Julia', last_name = 'Foldes', email = 'rfoldes1@odnoklassniki.ru', birthday = '2022-01-12'
    WHERE id = 2;
```
### Id'si 3 ve adı Tallia olan çalışanın last_name'i Jupiter olarak güncellendi
```sql
    UPDATE employee
    SET first_name = 'Tallia', last_name = 'Jupiter', email = 'tpatterfield2@va.gov', birthday = '2021-03-06'
    WHERE id = 3;
```
### Id'si 4 ve adı Hailey olan çalışanın birthday'i 2020.02.02 olarak güncellendi
```sql
    UPDATE employee
    SET first_name = 'Hailey', last_name = 'Illwell', email = 'hillwell3@hhs.gov', birthday = '2020.02.02'
    WHERE id = 4;
```
### Id'si 5 ve adı Gael olan çalışanın first_name'i Demo_demo ve last_name'i Test_test olarak güncellendi
```sql
    UPDATE employee
    SET first_name = 'Demo_demo', last_name = 'Test_test', email = 'ghaymes4@wired.com', birthday = '2021-02-10'
    WHERE id = 5;
```

<br>

## İstem → → Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
```sql
    DELETE FROM employee WHERE id = 9;
    DELETE FROM employee WHERE first_name = 'Grace';
    DELETE FROM employee Where last_name LIKE ('%a');
    DELETE FROM employee WHERE birthday = CURRENT_DATE;
    DELETE FROM employee WHERE  email ~ '[0-9]'
```
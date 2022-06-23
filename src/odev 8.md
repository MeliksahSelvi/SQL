# SQL SORGULARIMIZ

### 1.test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```
CREATE TABLE employee(
    
    id INTEGER NOT NULL,
    name VARCHAR(50) NOT NULL,
    birthday DATE,
    email VARCHAR(100)
);
```
### 2.Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
```
insert into employee (id, name, birthday, email) values (1, 'Correy', '2005-12-16', 'cvlach0@odnoklassniki.ru');
insert into employee (id, name, birthday, email) values (2, 'Jamie', '2006-11-30', 'jgilpin1@usatoday.com');
insert into employee (id, name, birthday, email) values (3, 'Riannon', '1988-05-21', 'rmothersole2@fotki.com');
insert into employee (id, name, birthday, email) values (4, 'Raymond', '2011-08-06', 'rmeredyth3@blogger.com');
insert into employee (id, name, birthday, email) values (5, 'Freddy', '1986-01-15', 'fnowick4@businesswire.com');
insert into employee (id, name, birthday, email) values (6, 'Sandra', '2016-09-09', 'skliner5@accuweather.com');
insert into employee (id, name, birthday, email) values (7, 'Cari', '2012-01-07', 'cvolonte6@networkadvertising.org');
insert into employee (id, name, birthday, email) values (8, 'Engelbert', '1972-11-04', 'ejakolevitch7@cmu.edu');
insert into employee (id, name, birthday, email) values (9, 'Janene', '1995-12-11', 'jreynoldson8@istockphoto.com');
insert into employee (id, name, birthday, email) values (10, 'Farlie', '2005-11-27', 'fkarlicek9@pen.io');
insert into employee (id, name, birthday, email) values (11, 'Shepperd', '1987-01-06', 'sbalcocka@hubpages.com');
insert into employee (id, name, birthday, email) values (12, 'Eleni', '1960-02-07', 'edrewellb@youtube.com');
insert into employee (id, name, birthday, email) values (13, 'Ludovika', '1994-04-08', 'lmacdwyerc@noaa.gov');
insert into employee (id, name, birthday, email) values (14, 'Sydel', '1955-04-09', 'ssherlandd@discovery.com');
insert into employee (id, name, birthday, email) values (15, 'Melly', '1983-06-20', 'mvearnalse@bbc.co.uk');
insert into employee (id, name, birthday, email) values (16, 'Stephine', '2017-11-17', 'shurlerf@jigsy.com');
insert into employee (id, name, birthday, email) values (17, 'Barth', '1987-05-09', 'bphilippoug@hud.gov');
insert into employee (id, name, birthday, email) values (18, 'Carmel', '2006-02-25', 'cpatrisksonh@joomla.org');
insert into employee (id, name, birthday, email) values (19, 'Val', '1993-05-13', 'vbowlesworthi@umn.edu');
insert into employee (id, name, birthday, email) values (20, 'Smith', '1952-08-07', 'sweyj@51.la');
insert into employee (id, name, birthday, email) values (21, 'Markos', '1994-06-15', 'mlunkk@army.mil');
insert into employee (id, name, birthday, email) values (22, 'Teodoro', '1960-08-20', 'trodgel@state.tx.us');
insert into employee (id, name, birthday, email) values (23, 'Maggi', '2010-08-20', 'manthoniesm@dyndns.org');
insert into employee (id, name, birthday, email) values (24, 'Hildegarde', '1971-06-25', 'hbockmannn@naver.com');
insert into employee (id, name, birthday, email) values (25, 'Lidia', '1993-10-10', 'ljermano@sciencedirect.com');
insert into employee (id, name, birthday, email) values (26, 'Filip', '2017-09-13', 'fseap@parallels.com');
insert into employee (id, name, birthday, email) values (27, 'Zak', '1956-07-02', 'zcurtissq@spiegel.de');
insert into employee (id, name, birthday, email) values (28, 'Noellyn', '1971-04-22', 'ndulyr@youku.com');
insert into employee (id, name, birthday, email) values (29, 'Bran', '2013-08-02', 'bciccottis@springer.com');
insert into employee (id, name, birthday, email) values (30, 'Amargo', '1998-06-20', 'aruzict@phoca.cz');
insert into employee (id, name, birthday, email) values (31, 'Selina', '1972-02-22', 'smcniffu@earthlink.net');
insert into employee (id, name, birthday, email) values (32, 'Chery', '1989-11-04', 'cmakeswellv@oaic.gov.au');
insert into employee (id, name, birthday, email) values (33, 'Andrej', '1998-06-16', 'adallaghanw@wisc.edu');
insert into employee (id, name, birthday, email) values (34, 'Lauree', '2002-10-31', 'lrastallx@comcast.net');
insert into employee (id, name, birthday, email) values (35, 'Tudor', '2008-04-28', 'tslateny@youtube.com');
insert into employee (id, name, birthday, email) values (36, 'Roxie', '2016-05-30', 'rwickershamz@ihg.com');
insert into employee (id, name, birthday, email) values (37, 'Oswell', '1954-09-11', 'obusfield10@angelfire.com');
insert into employee (id, name, birthday, email) values (38, 'Briano', '1951-04-09', 'bgounet11@fema.gov');
insert into employee (id, name, birthday, email) values (39, 'Tarrah', '1978-04-17', 'tknollesgreen12@cdbaby.com');
insert into employee (id, name, birthday, email) values (40, 'Kristan', '1968-07-23', 'kblennerhassett13@imgur.com');
insert into employee (id, name, birthday, email) values (41, 'Skyler', '2011-07-26', 'scosker14@hexun.com');
insert into employee (id, name, birthday, email) values (42, 'Raychel', '2016-03-12', 'rboosey15@google.es');
insert into employee (id, name, birthday, email) values (43, 'Lindsey', '1956-12-17', 'lgoshawke16@marriott.com');
insert into employee (id, name, birthday, email) values (44, 'Corliss', '1986-04-29', 'croggieri17@oracle.com');
insert into employee (id, name, birthday, email) values (45, 'Paddy', '1957-04-27', 'pgleasane18@opera.com');
insert into employee (id, name, birthday, email) values (46, 'Honey', '1972-08-04', 'hgye19@slideshare.net');
insert into employee (id, name, birthday, email) values (47, 'Gare', '2017-11-14', 'glagden1a@scientificamerican.com');
insert into employee (id, name, birthday, email) values (48, 'Jackelyn', '2004-10-24', 'jgrogan1b@ftc.gov');
insert into employee (id, name, birthday, email) values (49, 'Tucker', '1977-11-20', 'tdurrans1c@ning.com');
insert into employee (id, name, birthday, email) values (50, 'Almira', '1975-04-04', 'adragge1d@blogs.com');
```
### 3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
```
UPDATE employee
SET name='isim degisti.'
WHERE name LIKE('A%')
RETURNING *;
```
```
UPDATE employee
SET id='100'
WHERE id>45
RETURNING *;
```
```
UPDATE employee
SET birthday ='2022-06-23'
WHERE birthday='2004-10-24'
RETURNING *;
```
```
UPDATE employee
SET email ='meliksah.selvi2834@gmail.com'
WHERE email LIKE 'm%' OR  email LIKE 's%'
RETURNING *;
```
```
UPDATE employee
SET name='Jorce'
WHERE id BETWEEN 10 AND 15
RETURNING *;
```
### 4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
```
DELETE FROM employee
WHERE name='Jorce'
RETURNING *;
```
```
DELETE FROM employee
WHERE email='patika.dev@gmail.com'
RETURNING *;
```
```
DELETE FROM employee
WHERE birthday='2022-06-23'
RETURNING *;
```
```
DELETE FROM employee
WHERE id>50
RETURNING *;
```
```
DELETE FROM employee
WHERE id>30 AND name LIKE 'A%'
RETURNING *;
```

# Mini-Medical-Store
This is an java application for Medical Store that provide options like add or remove any Item, create and view Invoices etc.

## To run this project you need to create a Database"test" and 3 tables in it.

### Table 1: login

sql query for "login" table

create table login( id int NOT NULL AUTO_ICREMENT, usr varchar(100) NOT NULL, psw varchar(100) NOT NULL, PRIMARY KEY(id));

### Table 2: medicine

sql query for "medicine" table

create table medicine(id int NOT NULL AUTO_INCREMENT,name varchar(100), company varchar(100), fr varchar(200),price decimal,Sno int,PRIMARY KEY(id));

### Table 3: incoice

sql query for "invoice" table

create table invoice(id int,medicine varchar(1000),price decimal,name varchar(100),dt datetime,sno int NOT NULL AUTO_INCREMENT);

you need to aad a row in incoice table for proper working as there is AUTO_INCREMETN and crete table page accessing rows to generate a serialno for current invoice

#### example: insert into invoice(medicine,price,name,dt,sno) values('Crosine',2,'shub','12/8/2016',1000);

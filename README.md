# nkst
Enter password 'mysql'

Create database item;
use item;

create table student(grno int(5) primary key, Sname varchar(15) not null, phone int(13) unique);
TO show DECIMAL - Create table student(grno decimal(2,2));

insert into student values(102, "A", 1234567890);
insert into student values(103, "B", 1255567890);
insert into student values(104, "C", 1234577790);

Select* from student; 

Alter table student add column gender varchar(6);
Update student set gender="MALE";
Update student set gender "Female" Where grno=103 and grnp=104;
Select* from student;
alter table student modify grno int(10);
alter table student drop phone;
*indicates all records and fields.
delete from student;

Drop table student;
drop database item;
----------------------

To show start with 'a'
Select student where sname like"a%";
Select student where sname like "%b";

To set primary key 
Alter table tp
add constraint tp_pk
Primary key(grno);
--------------------

"Display ther total amount of each item. The amount must be calculated as price x quantity"

create database item;
use item;

create table item(itemno int(5) primary key, item name varchar(50), price int(5), quantity int(3) not null);

desc item;

insert into item values(1, "A", 2000, 2);
insert into item values(2, "B", 2005, 3);
insert into item values(3, "C", 2025, 4);
insert into item values(4, "D", 2153, 5);
insert into item values(5, "E", 1563, 6);

Select* from item;

select itemno, itemname, price, quantity, price*quantity as "amount" from item;

query2:_
Select* from item where price>2050;

Select* from item where price>2000 and price<2050;
---------------------------------------------------------

How can you check how many table are there in your database?

we will use show tables;

Ascending order:-
Select* from student order by sname;

Descending order:-
select* from student order by grno desc;
Select english+5 as "total" from student;

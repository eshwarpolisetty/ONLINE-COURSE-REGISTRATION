# ONLINE-COURSE-REGISTRATION
create table prof (
pname varchar(30),
p_id int,
p_email varchar(30));

create table registrar (
s_id int,
doconfirm date,
course varchar(30));

create table courses (
p_id int,
course varchar(30),
c_id int);

create table advisor (
s_id int,
course varchar(30),
c_id int,
pname varchar(30));

create table student ( 
fname varchar(30), 
lname varchar(30), 
uid int, 
s_id int, 
address varchar(50), 
phno int, 
email varchar(30));

insert into student
values ('anoushka','sanjeev',123,435,'anna nagar east',9884715940,'as5492@gmail.com');
insert into student
values ('polisetty','eshwar',456,598,'hyderabad',9003075113,'pe4932@gmail.com');
insert into student
values ('arumu','pm',789,174,'faridabad',7412386012,'ap3142@gmail.com');
insert into student
values ('ann','maraia',012,783,'kochi',9133819563,'am4232@gmail.com');
insert into student
values ('ann','phann',234,409,'guntur',861230412,'pa5212@gmail.com');
insert into student
values ('shiny','aby',567,305,'dubai',8135442663,'sa0222@gmail.com');

insert into registrar
values (435,'12-09-2023','math');
insert into registrar
values (568,'22-02-2022','chem');
insert into registrar
values (174,'13-10-2022','bio');
insert into registrar
values (783,'31-04-2023','eng');
insert into registrar
values (409,'11-06-2023','french');
insert into registrar
values (305,'30-02-2022','dbms');

insert into prof
values ('murugan',901,'muru@gmail.com');
insert into prof
values ('siva',783,'siva@gmail.com');
insert into prof
values ('velik',573,'veli@gmail.com');

insert into courses
values (901,'math','1032t');
insert into courses
values (901,'chem','203p');
insert into courses
values (783,'bio','723t');
insert into courses
values (573,'eng','e329');
insert into courses
values (573,'french','f433');
insert into courses
values (783,'dbms','p234');


insert into advisor
values (435,'math','1032t','murugan');
insert into advisor
values (568,'chem','203p','murugan');
insert into advisor
values (174,'bio','723t','siva');
insert into advisor
values (783,'eng','e329','velik');
insert into advisor
values (409,'french','f433','velik');
insert into advisor
values (305,'dbms','p234','siva');


Structured Query Language
Not Case-sensitive

DDL -> Data Definition Language (Create, Update, Alter, Truncate, comment and RENAME)
DML -> Data Manipulation Language (Insert, Update and Delete)
TCL -> Transaction control Language (COMMIT and ROLLBACK)
DCL -> Data Control Language (GRANT and REVOKE)


## Create Database

Create Database <db_name>;


## Create Table

Create Table <table_name>(
student_id int,
name varchar(255),
Address varchar(255),
City varchar(255)
);

Create Table <table_name_1> AS 
Select column1, column2,...
From <existing_table_name>
where ....;


## Insert 

insert into <table_name> values(value1,....);
or
insert into <table_name>(column1,column2)
values(value1,value2);

## Alter

Alter Table <table_name>
Add column_name datatype;

Alter Table <table_name>]
drop column column_name;

Alter Table <table_name_1>
Rename <new_table_name>;

Alter Table <table_name>
Rename column <old_name> to <new_name>;


## Primary key

Constraint PK_employees PRIMARY KEY(emp_id), -> when primary key is composite and named constraint


Alter table <name>
ADD constraint....;

Alter table  <name>
Drop Primary key;
or
drop constraint <name_pk>;


## Constraints

Unique
Not Null
Check
Default
Primary key
Foreign Key
Index


CHECK

age int,
check (age>0)
);

constraint name check (age>0 and sex='M')
);

Alter table <tb_name>
Drop check <name>

Alter table <tb_name>
Drop constraint <name>;




Auto Increment


Create table stud
{
student_id int not null auto_increment=1000;
}
start with 1000

Dates

Date - format YYYY-MM-DD
Datetime - format YYYY-MM-DD HH:M1:SS
Year - format YYYY or YY


SELECT

select emp_id from employees;

select distinct emp_id from employees;
select count(distinct branch_name) from employees;

where Between 1 and 3;

Not equal ->  <> in oracle

like -> pattern matching '%or%' or 'G_Y'

in -> present in given set (1,2,3)



ORDER BY

select * from employee where Dept=3
order by dept_name DESC



ASC -> Default


if nothing to differntiate on i.e, dept_name is same then first come in the table is first in the order

select * from employee where Dept=3 order by dept_name,Age DESC

prints all from employee table with dept 3 in ascending order to dept_name, when dept_name is same then Age is taken to priority in desc


UPDATE

update  <tb_name>
set column1=value1,column2=value2
where <condition>;


DELETE

delete from <tb_name>
where dept=3;


LIMIT 100 MySQL
FETCH FIRST 5 ROWS ONLY; -> Oracle

select min(salary)

if we give limit 1,1
first 1-> starting
second 1-> 1 after first one

ALIAS

select cust_name,Address+','+PostalCode+' '+city+','+Country as ADDRESS from customer;


GROUP BY
having is with group by (where for select is having for group by)

length () gives length
substr(str,start,number of letters from start)






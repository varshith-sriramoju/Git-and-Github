# SQL 01 Database and SQL Fundamentals

working with SQL with MySQL:
===========================

when we want to store the application users data , we will use  a

component called  "database" 

when we want to store the data in the database, based on how we 

store the data, the databases are classified into  two types: 
============================================================

1) relational database:
===================

when we store the data in the database in the form  of table, then the 

database is called as "relational database" 

in relational database, the data will be stored in the form of table ,

where the table will have the data in the form of  "rows and columns" 

where rows are also called as "records or tuples " 

where the columns are also called as "fields or attributes"  '

when we want to work with "relational database" , we are going to 

use a langauge called "SQL(sequel)" 

when we want to perform any operation on the "relational database" ,

then we are going to use "SQL" 

when we want to execute the "SQL query", we are going to use a

software called "DBMS" 

any DBMS we are using for "relational database", then the DBMS is

called as "relational DBMS (RDBMS)"

the popular RDBMS are: 

1) MySQL 

2) Oracle 

3) postgres SQL,..................... 

any SQL query we need to execute, we will always "use DBMS", 

in the DBMS will use a concept called "query Processor" and which is

responsible for "executing the SQL query" , query processor internally

uses a translator called "interpreter" 

in SQL, we will have the following sub-languages: 
==========================================

1)  Data Definition Language (DDL) :
================================

in this we will have the following commands: 
========================================================

1)  create:
=========

using this create command , we will do the following: 
=============================================

create the  "database | table | index | view | function | stored procedure

|.................." 
 

2)  rename 
=========

using this command "we can able to rename any table in the MySQL or 

any database object , we need to change the name , we will use 

rename 

3)  alter 
=======

when we create the table in MySQL, when we want to  do the following

, we will use the alter command :
============================================================

1)  add the new column in the existing table 

2)  remove the column in the existing table 

3)  rename the any column in the existing table  

4) change the any data type of the column in the existing table 

5) when we want to change name of the existing table 

4)  truncate 
===========

when we want to "remove the all rows of the table, in MySQL, we will

use truncate command" 

truncate command will never remove the "table structure", but remove

all rows of the table  

5)  drop 
=======

drop command is used in SQL, to "remove the database or view or 

table or index or  function or stored procedure" 

2)  Data Manipulation language (DML):
=================================

when we want to perform the operations on the table, we will use the 

following commands in SQL:

1)  Insert  (using this command we can able to insert rows into the 

  table) 

2)  update (using this command we can able to update the row in the 

table) 

3)  delete (using this command we can able to delete the row in the 

table)   

 

3)  Data Query Language (DQL)
===========================

when want to retrieve the data from the table, in sql, we will use a 

command called "select" 


4)  Data control Language (DCL) 
============================

when we want to give the access permissions to the users of the 

database, in SQL, we will use the following DCL commands:
===========================================================

1)  grant  (used to give the permissions to the users READ or Write) 

2) revoke(used to take back the given permissions from the users of 

                    the database)  


5) Transaction Control language (TCL)
=================================

all database operations can be done as "Transaction" 

when we want to work with transactions, in SQL, we will use the 

following TCL commands:
===========================================================

1) save point 

    save point used like a block, where the all operations are not effected

   directly onto the table, when we perform any operation on the 

   database  tables, those operation will effect only when we save 

    the operation 

2) commit 

     commit is used to  "save the operation permanently on  the table"

3) rollback 

    rollback is used to perform "undo" operation 

when we want to create the database in MySQL, we will use 

following syntax: 

           create database database_name; 

example: 

create database employee_fp2_3_2026; 

create database hr_2026; 

create database student_2026; 

when we want to show the all available databases in the MySQL, we 

will use the following syntax: 

                   show databases; 

when we want to create any table, when we want work with any table

inside the database, then we will always "set the database as current 

database", to set the database "current database", then we will use

the following syntax MySQL: 

                    use database_name; 

when we want to know the "what is current database", in the MySQL ,

we will use the following syntax: 
============================================================

                           select database() ;

when we want to create the table in the MySQL database, we will use 

the following syntax: 

create table table_name(col_name datatype constraint, 

col_name datatype constraint, col_name data_type constraint,

.
.
.
coln datatype constraint)

here data type refers "What type of data, the column can have or can 

store, we need to specify while creating the table" , while inserting 

data, MySQL query processor  will check given data as per the "given 

data type of column"  or not
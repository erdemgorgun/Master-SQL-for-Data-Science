# Master-SQL-for-Data-Science
## 1. DATABASE BASICS
### 1.1.What is a Database
Corporation’s most valuable asset besides employees and customers is data. Most critical decisions made by business come form analyzing lots of data. The data could be related to several areas. Without data analysis, companies work without a direction or strategy. Ads are offered based on your purchasing history. Companies like facebook, amazon collect data of customer and offer customized ads. The data is saved in database. This course shows how to extract critical insight from data that is saved in a relational database.

Database is a collection of tables. Most of database experience is related to deal with working with tables. Tables contain actual data. This course help me master how to get insight from data. To be a master, I need secure skill which is called SQL (Structured Query Language). This language can be related also other databases.

![Untitled](https://user-images.githubusercontent.com/99462935/161200289-e8c8af98-553b-4a37-acb4-364853de1c8b.png)

In a table each column contains an information of same data type. Horizontally each row collects data of a supplier, employee, etc. If a table is supplier table, it should only consists supplier information.
Download Postgress to run SQL queries in this training.
### 1.2.Create Table and Insert Statements
PJI admin connect database but database does not store data. Data is stored in table. In this lecture, we create a table and then insert data into that table. SQL that will be typing into out PJI admin tool to create and insert tables. SQL is used to both creating and analyzing the data. In each column of table, there can be set restriction about data type (numbers, English characters, etc.). A table structure is defined by using SQL statements. Constraints can be set in SQL. Constraint is basically the databas’s ability to control what kind of data goes in a given column. In SQL,  create a table and  create columns (Ex: department varchar(100)). Primary key (department) prevents us from entering department two times (accept it once) or empty data (null). To insert data into table, use insert statement. For example “insert into departments values (‘Automotive’, ‘Auto & Hardware’);” code that insert first value goes into first column, and second value goes into second column. ’Automotive’ data cannot be used again since primary key does not allow to use it twice. Primary key can be define only once. But it can be defined for multiple columns. SQL includes statements such as creating the table ‘departments’. Statement ends with semicolumn (Ex: create or insert statement). When a column is created, there is another attribute nex to it. This is data type such as int or varchar. Int refers to integer and varchar symbolize character. Varchar(20) limits that number of characters should be less than 20. First create a table then insert data into this table. Script should be followed step by step.
### 1.3.Prepare the Database
mock-data.txt is downloaded. Copy the first statement. New database is created in PostgreSQL. Click on Tools and select Query Tool.  We wll use mostly this interface to write SQL commands. Paste first statement into Query Tool.

create table departments (
department varchar(100),
division varchar(100),
primary key (department)
);

If we try to write "prima key" instead of "primary key" it gives error in message tab.
![Untitled (1)](https://user-images.githubusercontent.com/99462935/161200883-9583b189-5d1a-4093-a064-0e1e6776a897.png)

Delete first statement and insert data for the column. Select all column and click Run. It succesfully run. Do this for other statements and run that statements. After run the statements run the code "SELECT * FROM employees" to see the employee table.

![Untitled (2)](https://user-images.githubusercontent.com/99462935/161201197-2ae8c4d3-73dd-4bf0-9942-58cf3e6a8216.png)

First row also gives data type. **Data scientist must understand the data.** To understand the data write SQL statements and understand the data. PostgreSQL only runs the statement that is selected. 

region_id in employee table comes from the options region_id of region table. %80 of the time as a data scientist is related to select from commands.

### Assignment 1: Create More Tables and Populate Data
![Untitled (3)](https://user-images.githubusercontent.com/99462935/161201431-164e4df5-f879-4706-9140-033174f74832.png)

Datatypes are varchar, integer and date

The datatype of course_no column is character with maximum 5 letter.

Student enrollment has 2 columns. 

Teach table has 8 rows.


# Read: Class 9 : SQL

- - -

## SQL Bolt

> Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications. Relational databases
 


### popular SQL databases 

 **SQLite** , **MySQL**, **Postgres**, **Oracle** and Microsoft SQL Server.

All of them support the common SQL language standard, which is what this site will be teaching, but each implementation can differ in the additional features and storage types it supports.    


A **relational database** represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data. In such a database, you might find additional related tables containing information such as a list of all registered drivers in the state, the types of driving licenses that can be granted, or even driving violations for each driver.    


### SELECT queries 101 

To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned. It has a specific syntax though, which is what we are going to learn in the following exercises.     

* Select query for a specific columns    
  `SELECT column, another_column, …`    
  `FROM mytable;`

The result of this query will be a two-dimensional set of rows and columns, effectively a copy of the table, but only with the columns that we requested.     


* If we want to retrieve absolutely all the columns of data from a table, we can then use the asterisk (*) shorthand in place of listing all the column names individually.    

  * Select query for all columns    

  `SELECT * `    
  `FROM mytable;`
 



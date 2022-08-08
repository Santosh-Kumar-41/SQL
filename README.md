# SQL (Structured Query Language)

To mange relational database and perform various on the data in them we use SQL, which is a standardized programming language.Initially created in the 1970s, SQL is regularly used not only by database administrators, but also by developers writing data integration scripts and data analysts looking to set up and run analytical queries.

# Why Is SQL Popular?

The data trail we create every single day as we jump between apps, sites and social platforms is being mined by companies for various uses. But data in its raw form is useless without data analysts.

These professionals use programming languages like SQL to organize and analyze large data sets. In doing so, they’re able to derive information and correlations that can be turned into business insights, which in turn can help companies grow their business. As this pile of data grows larger by every passing second, so too does the demand for people who are skilled in SQL.

# A Few Good Reasons to Master SQL

Before you invest time in learning SQL, you probably want to be certain that it’s going to be worthwhile. We’ve put together a list below of the top reasons why learning S

* You can manage vast pools of data – For years, spreadsheets were the go-to method to store and analyze data sets, but they could be restrictive when it came to handling large pools of data.


* SQL is easy to pick up – SQL’s basic commands are easy to retain and utilize as they’re quite similar to the English language. Commands like INSERT, DELETE, and UPDATE are obviously rooted in our everyday language.


* You’ll find the right information fast– A person well-versed in SQL can, in a matter of seconds, pull up relevant information from enormous data sets by just tweaking the queries within the program.


* SQL is a powerful troubleshooting tool – SQL makes it incredibly easy for you to troubleshoot any issues that might crop up in daily use. A simple syntax error or misplaced indicator that might normally go by unnoticed is highlighted by the program.


* SQL is very versatile – SQL has now crept into almost all business fields as the world becomes more reliant on computing. Finance, social media enterprises, data analytics firms, scientific computing, website and game development.


* SQL is standardized – SQL, as mentioned, has been around for almost 41 years now and is not likely to go anywhere for the next few decades, seeing how relevant it still is.


* SQL developers are paid well – In 2020, Glassdoor listed the average pay for a SQL developer as $81,000, steeper than many other salary packages being offered in the tech industry. Proprietary and open source relational database management systems built around SQL are available for use by organizations. They include:


* Microsoft SQL Server


* Oracle Database


* IBM DB2


* SAP HANA


* SAP Adaptive Server


* MySQL (now owned by Oracle)


* PostgreSQL


# SQL Process

When you want to execute an SQL command for any DBMS system, you need to find the best method to carry out your request, and SQL engine determines how to interpret that specific task.

Important components included in this SQL process are:

  * SQL Query Engine

  * Optimization Engines

  * Query Dispatcher

  * Classic Query Engine

A classic query engine allows you to manage all the non-SQL queries.

![sql-map](https://camo.githubusercontent.com/827702d8c0f9331b7e97bb45468cb62401c95f1dfeefc1ee817fe79cf013ac61/68747470733a2f2f7777772e6775727539392e636f6d2f696d616765732f73716c2d7475746f7269616c2e706e67)


# Understanding the SQL Commands

![sql-map](https://camo.githubusercontent.com/2fc21692048dcae7f9b59488d4a16bf003ab706924fcda6c819c86e1cfd25f1d/68747470733a2f2f3134393639353834372e76322e707265737361626c6563646e2e636f6d2f77702d636f6e74656e742f75706c6f6164732f323031392f30362f746162652e706e67)

**Data Definition Language (DDL)**:The DDL commands such as create, drop, alter and truncate is used for creating, dropping, altering and modifying the structure of database objects.

**Data Manipulation Language (DML)**:The DML commands such as insert, update and delete are used for inserting, updating and deleting the structure of database objects.

**Data Control Language (DCL)**:The DCL commands such as grant and revoke are used for providing security to database objects.

**Data Query Language (DQL)**:The DQL command such as select is used for retrieving data from the database.

**Transaction Control Language (TCL)**:TCL commands such as commit, rollback and savepoint is used for managing transactions in the database.

# SQL Commands: Data Definition Language Commands (DDL)

## 1. CREATE

This statement is used to create a table or a database.

### 1.1 The CREATE DATABASE Statement

As the name suggests, this statement is used to create a database.
 ```    
     CREATE DATABASE Employee;
```

### 1.2 CREATE TABLE

CREATE TABLE creates a new table inside a database.

      CREATE TABLE customers (
          customer_id int,
          name varchar(255),
          age int
       );
       

## 2. DROP

This statement is used to drop an existing table or a database.

### 2.1 The DROP DATABASE Statement

This statement is used to drop an existing database. When you use this statement, complete information present in the database will be lost.

```
    DROP DATABASE dataquestDB;
```

### 2.2 The DROP TABLE Statement

This statement is used to drop an existing table. When you use this statement.

  ```    
     DROP TABLE customers;
   ```
## 3. ALTER

This command is used to delete, modify or add constraints or columns in an existing table.

### 3.1 The ALTER Statement

This statement is used to add, delete, modify columns in an existing table. The

### 3.2 ALTER TABLE Statement with ADD/DROP COLUMN

You can use the ALTER TABLE statement with ADD/DROP Column command according to your need. If you wish to add a column, then you will use the ADD command, and if you wish to delete a column, then you will use the DROP COLUMN command.

```
     ALTER TABLE TableName
     ADD ColumnName Datatype;

     ALTER TABLE TableName
     DROP COLUMN ColumnName;
```

## 4. TRUNCATE

This command is used to delete the information present in the table but does not delete the table.
```
     TRUNCATE TABLE TableName;
```
# SQL Commands: Data Manipulation Language Commands (DML)

This section of the article will give you an insight into the commands through which you can manipulate the database. The commands are as follows:

## 1. INSERT INTO

This statement is used to insert new records into the table.
```
     INSERT INTO table_name (column1, column2, column3, ...)
     VALUES (value1, value2, value3, ...); 
```

## 2. UPDATE

The UPDATE statement is used to update data in a table. For example, the code below would update the age of any customer named Bob in the customers table to 56.
```
     UPDATE customers
     SET age = 56
     WHERE name = ‘Bob’;
```

## 3. DELETE

```
     DELETE FROM customers
     WHERE name = ‘Bob’;
```

# SQL Commands: Data Control Language Commands (DCL)

This section of the article will give you an insight into the commands which are used to enforce database security in multiple user database environments. The commands are as follows:

## 1. GRANT

This command is used to provide access or privileges on the database and its objects to the users.

```
     GRANT PrivilegeName
     ON ObjectName
     TO {UserName |PUBLIC |RoleName}
     [WITH GRANT OPTION];
```
## 2. REVOKE

This command is used to withdraw the user’s access privileges given by using the GRANT command.

```
     REVOKE PrivilegeName 
     ON ObjectName 
     FROM {UserName |PUBLIC |RoleName}
```

# SQL Commands: Data Query Language (DQL):

The DQL command such as select is used for retrieving data from the database. The commands are as follows:

## 1. SELECT

SELECT is probably the most commonly-used SQL statement. You’ll use it pretty much every time you query data with SQL. It allows you to define what data you want your query to return.
```
     SELECT name
     FROM customers;

     SELECT * FROM customers;
```

# SQL Commands: Transaction Control Language Commands (TCL)

This section of the article will give you an insight into the commands which are used to manage transactions in the database. The commands are as follows:

## 1. COMMIT

This command is used to save the transaction into the database.
```
     COMMIT;
```

## 2. ROLLBACK

This command is used to restore the database to the last committed state.
```
     ROLLBACK
```

## 3. SAVEPOINT

This command is used to temporarily save a transaction. So if you wish to rollback to any point, then you can save that point as a ‘SAVEPOINT’.
```
     SAVEPOINT SAVEPOINTNAME;
```

# SQL JOIN

A JOIN clause is used to combine rows from two or more tables, based on a related column between them.

## 1. INNER JOIN

INNER JOIN selects records that have matching values in both tables.
```
     SELECT name
     FROM customers
     INNER JOIN orders
     ON customers.customer_id = orders.customer_id;
```

## 2. LEFT JOIN

LEFT JOIN selects records from the left table that match records in the right table. In the below example the left table is customers.
```
     SELECT name
     FROM customers
     LEFT JOIN orders
     ON customers.customer_id = orders.customer_id;
```

## 3. RIGHT JOIN

RIGHT JOIN selects records from the right table that match records in the left table. In the below example the right table is orders.
```
     SELECT name
     FROM customers
     RIGHT JOIN orders
     ON customers.customer_id = orders.customer_id;
```

## 4. FULL JOIN

FULL JOIN selects records that have a match in the left or right table. Think of it as the “OR” JOIN compared with the “AND” JOIN (INNER JOIN).
```
     SELECT name
     FROM customers
     FULL OUTER JOIN orders
     ON customers.customer_id = orders.customer_id;
```

## 5. SQL SELF JOIN

A self join is a regular join, but the table is joined with itself.
```
     SELECT column_name(s)
     FROM table1 T1, table1 T2
     WHERE condition;
```

# SQL Aggregation:

SQL aggregation is the task of collecting a set of values to return a single value. It is done with the help of aggregate functions, such as SUM, COUNT, and AVG. For example, in a database of products, you might want to calculate the average price of the whole inventory.

### How is it used?

Aggregation in SQL is, typically, used in conjunction with grouping. The Group By clause is used to arrange rows into groups in SQL. Aggregation, together with grouping, is key to generating quick reports and insights from a database. For example, an ecommerce company might want to see its highest spending customers over a given time period.

### Aggregate Functions

This section of the article will include the following functions:

  * MIN()
  * MAX()
  * COUNT()
  * SUM()
  * AVG()

## 1. MIN Function

The MIN function returns the smallest value of the selected column in a table.
```
     SELECT MIN(ColumnName)
     FROM TableName
     WHERE Condition;
```

## 2. MAX Function

The MAX function returns the largest value of the selected column in a table.
```
     SELECT MAX(ColumnName)
     FROM TableName
     WHERE Condition;
```

## 3. COUNT Function

The COUNT function returns the number of rows which match the specified criteria.
```
     SELECT COUNT(ColumnName)
     FROM TableName
     WHERE Condition;
```

## 4. SUM Function

The SUM function returns the total sum of a numeric column that you choose.
```
     SELECT SUM(ColumnName)
     FROM TableName
     WHERE Condition;
```

## 5. AVG Function

The AVG function returns the average value of a numeric column that you choose.
```
     SELECT AVG(ColumnName)
     FROM TableName
     WHERE Condition;
```

# SQL Commands: Different Types Of Keys In Database

There are mainly 7 types of Keys, that can be considered in a database. I am going to consider the below tables to explain to you the various keys.

![sql-map](https://camo.githubusercontent.com/5e42e98f1863bda6c479ec65790db999e7b7e59ba3637854a20695df11d9e99a/68747470733a2f2f64316a6e783962613873366a39722e636c6f756466726f6e742e6e65742f626c6f672f77702d636f6e74656e742f75706c6f6164732f323031392f30332f446966666572656e742d54797065732d6f662d4b6579732d53514c2d436f6d6d616e64732d45647572656b612e706e67)

*   **Candidate Key** - A set of attributes which can uniquely identify a table can be termed as a Candidate Key. A table can have more than one candidate key, and out of the chosen candidate keys, one key can be chosen as a Primary Key. In the above example, since EmployeeID, InsuranceNumber and PanNumber can uniquely identify every tuple, they would be considered as a Candidate Key.


*  **Super Key** - The set of attributes which can uniquely identify a tuple is known as Super Key. So, a candidate key, primary key, and a unique key is a superkey, but vice-versa isn’t true.


*  **Primary Key** - A set of attributes which are used to uniquely identify every tuple is also a primary key. In the above example, since EmployeeID, InsuranceNumber and PanNumber are candidate keys, any one of them can be chosen as a Primary Key. Here EmployeeID is chosen as the primary key.


*  **Alternate Key** - Alternate Keys are the candidate keys, which are not chosen as a Primary key. From the above example, the alternate keys are PanNumber and Insurance Number.


*  **Unique Key** - The unique key is similar to the primary key, but allows one NULL value in the column. Here the Insurance Number and the Pan Number can be considered as unique keys.


* **Foreign Key** -  An attribute that can only take the values present as the values of some other attribute, is the foreign key to the attribute to which it refers. in the above example, the Employee_ID from the Employee_Information Table is referred to the Employee_ID from the Employee_Salary Table.


* **Composite Key** - A composite key is a combination of two or more columns that identify each tuple uniquely. Here, the Employee_ID and Month-Year_Of_Salary can be grouped together to uniquely identify every tuple in the table.


## Reference and Resources

  * https://docs.oracle.com/en/database/oracle/oracle-database/21/cncpt/sql.html#GUID-DA48618A-A6BB-421A-A10A-02859D8ED9AD

  * https://www.geeksforgeeks.org/sql-ddl-dql-dml-dcl-tcl-commands/?ref=lbp

  * https://bookdown.org/paranedagarcia/database/sql.html

  * https://www.geeksforgeeks.org/query-execution-engine-in-sql

  * https://www.javatpoint.com/dbms-sql-command














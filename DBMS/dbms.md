# DBMS
* important link:https://www.interviewbit.com/sql-interview-questions/
## Subquery
### Non correlated subquery
* In non correlated subquery, inner query doesn't depend on outer query and can run as stand alone query.Subquery used along-with IN or NOT IN sql clause is good examples of Noncorrelated subquery in SQL.
* NonCorrelated subquery are used along-with IN and NOT IN clause.
### Correlated subquery
* Correlated subqueries are the one in which inner query or subquery reference outer query. Outer query needs to be executed before inner query. One of the most common example of correlated subquery is using keywords exits and not exits. An important point to note is that correlated subqueries are slower queries and one should avoid it as much as possible.
### Difference between Correlated and NonCorrelated Subquery
* In case of correlated subquery inner query depends on outer query while in case of noncorrelated query inner query or subquery doesn't depends on outer query and run by its own.
* In case of correlated subquery, outer query executed before inner query or subquery while in case of NonCorrelated subquery inner query executes before outer query.
* Correlated Sub-queries are slower than non correlated subquery and should be avoided in favor of sql joins.
* Common example of correlated subquery is using exits and not exists keyword while non correlated query mostly use IN or NOT IN keywords.
### SubQuery vs Join in SQL
* Any information which you retrieve from database using subquery can be retrieved by using different types of joins also. Since SQL is flexible and it provides different way of doing same thing. Some people find SQL Joins confusing and subquery specially noncorrelated more intuitive but in terms of performance SQL Joins are more efficient than subqueries.
### Important points about SubQuery in DBMS
* Almost whatever you want to do with subquery can also be done using join, it just matter of choice
subquery seems more intuitive to many user.
* Subquery normally return an scaler value as result or result from one column if used along with
IN Clause.
* You can use subqueries in four places: subquery as a column in select clause,
* In case of correlated subquery outer query gets processed before inner query.

### What are UNION, MINUS and INTERSECT commands?
* The UNION operator combines and returns the result-set retrieved by two or more SELECT statements.
* The MINUS operator in SQL is used to remove duplicates from the result-set obtained by the second SELECT query from the result-set obtained by the first SELECT query and then return the filtered results from the first.
* The INTERSECT clause in SQL combines the result-set fetched by the two SELECT statements where records from one match the other and then returns this intersection of result-sets.

### Certain conditions need to be met before executing either of the above statements in SQL:
* Each SELECT statement within the clause must have the same number of columns
* The columns must also have similar data types
* The columns in each SELECT statement should necessarily have the same order

## What is a View?
A view in SQL is a virtual table based on the result-set of an SQL statement. A view contains rows and columns, just like a real table. The fields in a view are fields from one or more real tables in the database.

## SQL vs NoSQL
* Structured Query language (SQL) pronounced as "S-Q-L" or as "See-Quel" is the standard language
* NoSQL is a non-relational DMS, that does not require a fixed schema, avoids joins, and is easy to scale

### Scalibility
* With horizontal-scaling it is often easier to scale dynamically by adding more machines into the existing pool — Vertical-scaling is often limited to the capacity of a single machine, scaling beyond that capacity often involves downtime and comes with an upper limit.

### ACID vs. BASE Model
* ACID( Atomicity, Consistency, Isolation, and Durability) is a standard for RDBMS
* Base ( Basically Available, Soft state, Eventually Consistent) is a model of many NoSQL systems

### When use SQL?
* SQL is the easiest language used to communicate with the RDBMS
* Analyzing behavioral related and customized sessions
* Building custom dashboards
* It allows you to store and gets data from the database quickly
* Preferred when you want to use joins and execute complex queries

### When use NoSQL?
* When ACID support is not needed
* When Traditional RDBMS model is not enough
* Data which need a flexible schema
* Constraints and validations logic not required to be implemented in database
* Logging data from distributed sources
* It should be used to store temporary data like shopping carts, wish list and session data

## Clustered vs Non-clustered Index
### What is an Index?
An Index is a key built from one or more columns in the database that speeds up fetching rows from the table or view. This key helps a Database like Oracle, SQL Server, MySQL, etc. to find the row associated with key values quickly.

# Build and Destroy: Introductory SQL Queries

Given the scenarios, add the the directed queries to the "answers" directory's files.

## Creating databases

Write the correct SQL statement to create a new database called **myNewDB**.

*(Add your query to the file exercise1.sql)*
mysql> CREATE SCHEMA myNewDB;

## Deleting databases

Write the correct SQL statement to delete a database named **myNewDB**.

*(Add your query to the file exercise2.sql)*
DROP SCHEMA myNewDB;

## Creating tables

Write the correct SQL statement to create a new table called **Users**, with an int field called **UserID**, and the following varchar fields of size 255: **LastName, FirstName, Address, City**

*(Add your query to the file exercise3.sql)*
CREATE TABLE myNewDB.Users ( UserID int, LastName varchar(255), FirstName varchar(255), Address varchar(255), City varchar(255) );

## Deleting tables

Write the correct SQL statement to delete a table called **Users**.

*(Add your query to the file exercise4.sql)*
mysql> DROP TABLE myNewDB.Users;


Use the **TRUNCATE** statement to delete all data inside the **Users** table.

*(Add your query to the file exercise5.sql)*
mysql> TRUNCATE myNewDB.Users;

## Altering tables

Add a column of type **DATE** called **Birthday** to the **Users** table.

*(Add your query to the file exercise6.sql)*
ALTER TABLE myNewDB.Users
    -> ADD Birthday DATE;

Delete the column **Birthday** from the **Users** table.

*(Add your query to the file exercise7.sql)*
  ALTER TABLE myNewDB.Users
    -> DROP COLUMN Birthday;


## Inserting records

Insert a new record in the **Students** table.

**Schema:**
 
```
StudentName,
Address, 
City, 
PostalCode,
Country
```

**Record's info to enter:**

```
Jane Doe
57 Union St
Glasgow, Scotland
G13RB
```

*(Add your query to the file exercise8.sql)*

## Selecting Records

### Where

Use the **NOT** keyword to select all records in the **Students** table where **City** is NOT "Philadelphia".

*(Add your query to the file exercise9.sql)*

Select all records in the **Students** table where the **City** column has the value 'Philadelphia' or 'Trenton'.

*(Add your query to the file exercise10.sql)*

### Order By
Select all records from the **Students** table, sort the result alphabetically by the column **City**.

*(Add your query to the file exercise11.sql)*

Select all records from the **Students** table, sort the result reversed alphabetically by the column **City**.

*(Add your query to the file exercise12.sql)*

Select all records from the **Students** table, sort the result alphabetically, first by the column **Country**, then by the column **City**.

*(Add your query to the file exercise13.sql)*

### Null values
Select all records from the **Students** where the **PostalCode** column is empty.

*(Add your query to the file exercise14.sql)*

Select all records from the **Students** where the **PostalCode** column is **NOT** empty.

*(Add your query to the file exercise15.sql)*


## Updating records
Update the **City** column of all records in the **Students** table and set it to "Edinburgh".

*(Add your query to the file exercise16.sql)*
 
 Set the value of the **City** columns to "Edinburgh", but only the ones where the **Country** column has the value "Scotland".

*(Add your query to the file exercise17.sql)*
 
Update the **City** value and the **Country** value to "Edinburgh", "Scotland" in the **Students** table, for the Student whose ID is 35.

*(Add your query to the file exercise18.sql)*

## Deleting Records
Delete all the records from the **Students** table where the **Country** value is "Scotland".

*(Add your query to the file exercise19.sql)*
 
Delete all the records from the **Students** table.

*(Add your query to the file exercise20.sql)*

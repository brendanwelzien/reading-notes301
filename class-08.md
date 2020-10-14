# SQL
What is *SQL*?
    - structured query language, designed to allow users to manipulate / transform data from a relational database
    - provides storage for websites and applications
- important to understand relational databases

## Selecting Queries
- to retrieve data from SQL database, you need to write *SELECT* statements, referred as queries
    - declares what data we are looking for, where to find it, and how to transform it
```bash
SELECT COLUMN, ..... , 
FROM mytable
```
- if you want to retrieve all items from something use the *asterik*

## Queries with Constraints
- in order to filter out specific colums of data, we need to use a *WHERE* statement
```bash
SELECT column, .... ,
FROM my table
WHERE condition
    AND / OR another_condition
    AND / or ..
```
 - more complex clauses can be creaetd by joining *AND* *OR* 
    - BETWEEN...AND..
    - NOT BETWEEN...AND..
    - IN (...)
    - NOT IN (...)
    - LIKE
    - NOT LIKE
    - %

## Filtering and Sorting Out Query Results
- SQL provides *DISTINCT* keyword by discarding rows with duplicate column values
- sometimes column orders are messy, so it can be difficult to read through, you can sort results by using *ORDER BY*
- *LIMIT* and *OFFSET* indicates the subset of the results you want

## Inserting Rows
- What is a schema? It describes the structure of each table, and datatypes that each column of the table can contain
    - when inserting new data, we need to use the *INSERT* statement, this declares where to write into
```bash
INSERT INTO mytable
VALUES (..., ...., ....,)
```
## Updating Rows
- to update use the *UPDATE* keyword... You have to specify which places you want to update as well
```bash
UPDATE my table
SET column = value
WHERE condition
```
- it is helpful to use the *SELECT* statement first to assure you are updating the correct areas of the database

## Deleting Rows
- use *DELETE* statement for the table to act upon, and for the rows of the table through the *WHERE* keyword
    - if you leave out the *WHERE* keyword, all the rows are removed... run contstraint through *SELECT* first

## Creating Tables
- use *CREATE TABLE* statement
```bash
CREATE TABLE IF NOT EXISTS mytable(
    column DataType TableConstraint DEFAULT....
)
```
- INTEGER, BOOLEAN	
The integer datatypes can store whole integer values like the count of a number or an age. In some implementations, the boolean value is just represented as an integer value of just 0 or 1.

- FLOAT, DOUBLE, REAL
The floating point datatypes can store more precise numerical data like measurements or fractional values. Different types can be used depending on the floating point precision required for that value.

- CHARACTER(num_chars), VARCHAR(num_chars), TEXT
The text based datatypes can store strings and text in all sorts of locales. The distinction between the various types generally amount to underlaying efficiency of the database when working with these columns.

Both the CHARACTER and VARCHAR (variable character) types are specified with the max number of characters that they can store (longer values may be truncated), so can be more efficient to store and query with big tables.

- DATE, DATETIME
SQL can also store date and time stamps to keep track of time series and event data. They can be tricky to work with especially when manipulating data across timezones.
- BLOB
Finally, SQL can store binary data in blobs right in the database. These values are often opaque to the database, so you usually have to store them with the right metadata to requery them.

## Altering Tables
- use the *ALTER TABLE* statement
- you need to specify the data type along with other constraints, you can specify where to insert new column by using *FIRST* or *AFTER*
    - removing columns by using the *DROP* method, or if you need to rename use the *RENAME* method
[<=Back](README.md)
# Database Normalization
- database normalization is the process of organizing tables and columns in a way where repetitive data can be avoided
    - limit a table to one purpose so you can reduce the number of duplicate data

*Reasons to normalization databases*
1. minimize duplciate data
2. minimize or avoid data modification issues
3. simplify queries
    
    - setbacks include...
    - increased storage and decreased performance
    - more difficult to maintain data changes
    - search/sort issues with separating and narrowing data

## Forms of Databse Normalization
- 1st, 2nd, 3rd, these forms are progressive, so for the 3rd form to work the 2nd and 1st form must work as well
    - 1st: information stored in a relational table with each column containing 'atomic' values.. There are no repeating groups of columns
    - 2nd: table is in first normal form and columns depend on table's primary key
    - 3rd: the table is in 2nd normal form and columns are no dependent on primary key
[<=Back](README.md)
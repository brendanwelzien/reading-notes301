## SMACCS
Base: for single element styles
layout: structural elements

```html
<!DOCTYPE html>
<html>
<head>
<!-- meta info and dependency management -->
<title></title>
<link>
</head>
<body></body>
</html>
```
- this is the basic html shell you must know

- header, main, and footer are layout/ structural components
- h1, p are generic single elements - base styles apply here
- section is meant for specific content within layout structure, or 'module'

- media queries

# Promises
*resolved*
    .then()

*pending*
- the midpoint state before it is either resolved or rejected

*rejected*
    .catch()

# SQL & Caching
- Database can be used for caching requests made by the user
    - client --> server --> API --> server --> (save) database --> server --> client (this is first request)
    - 2nd request you do not need to go through APIs again, you can bypass that and go to DB 
- REST: POST, GET, PUT, DELETE --> managed through app.get, etc. (INTERNET) works hand in hand as a model with CRUD
    ## CRUD
    - CRUD: CREATE, READ, UPDATE, DELETE/DESTROY (DATABASE)
    Persistence: web applications need a way to store data, this process is also called *persistence*
        - typically on the server, but can also be in the browser (*localstorage*)
    ## DATABASE
    - DBMS is a management system for databases that contain tables of data
    - a tool to the hold the data until we grab it
- SQL statements are made up of clauses, exressions, and predicates for inserting, retrieving, updating, and deleting data
    - special-purpose programming language designed for managing data
- queries retrieve data from one+ tables, or expressions
    - i make a request to the server, then to the database, then hand it off back to the client
    
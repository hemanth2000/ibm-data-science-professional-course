# Databases and SQL for Data Science

Main content:

1. Learned about basics of SQL
1. Relational databases

Sequential Query Language(SQL) is used for writing queries for a relational database to retrieve information from it.

Data : Collection of information in the form of words, numbers, pictures etc.

Database : Repository of data. Provides functionalities such as adding, deleting, and quering data.

Databases are classified based on the way they store data.

1. Relational database: Stores data in tabular form

   Ex: MySQL, Oracle Database, IBM Db2, etc.

2. Non-relational database

There are mainly five basic SQL commands.

1. Create a table
1. Insert
1. Select
1. Update
1. Delete

### Select Statement

A data manipulation language statement used to read and modify the data.

**Syntax**

```SQL

    Select * from <tablename>

        WHERE predicate


```

### COUNT

Counts the number of records in the database that satisfies the query.

```SQL

    Select COUNT(COUNTRY) from MEDALS

        where COUNTRY = 'INDIA'
```

### DISTINCT

Counts the number of distinct records in the database

```SQL

    Select DISTINCT columnnames from tablename

```

### LIMIT

Restricts the number of rows of the query.

```SQL

    Select * from MEDALS LIMIT 10

```

### INSERT

```SQL

    INSERT INTO tablename

        (column1, column2, column3,...)
        VALUES
        (val1,val2,val3,...)

```

### UPDATE & DELETE

```SQL

    UPDATE[TABLENAME]
    SET[[ColumnName]=[Value]]
    <WHERE[Condition]>

    DELETE FROM [TABLENAME]
        WHERE[CONDITION]
```

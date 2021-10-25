# Databases and SQL for Data Science

## Week 1: SQL Basics

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

## Week 2: RDB Concepts

Advantages of Relational Databases:

1. Data independence
2. Entities are independent objects which have attributes
3. Entities are mapped as rows in a table
4. Attributes are mapped as columns
5. A primary key uniquely identifies a specific row in a table.
6. Common data types include characters, numbers, and dates/times.

### Creating database instance on cloud

Some of the cloud based RDB are:

1. IBM Db2
1. Databases for PostgreSQL
1. Oracle Database Cloud Services
1. Microsoft Azure SQL Database
1. Amazon Relational Database Services (RDS) etc.

### DDL vs DML statements

Data Definition Language statements: Define, change, or drop tables(objects).

    Common DDL operations: CREATE, ALTER, TRUNCATE

Data Manipulation Language statements: Read and modify data. These are also known as CRUD operations.

    Common DML operations: INSERT, SELECT, UPDATE, DELETE

**DDL STATEMENTS:**

### CREATE

```SQL

    CREATE TABLE table_name
        (
            column_name_1 datatype optional_parameters,
            column_name_2 datatype,
            ...
            column_name_n datatype
        )
```

### ALTER, TRUNCATE

```SQL

    ALTER TABLE table_name

        ADD COLUMN column_name datatype


    ALTER TABLE table_name

        ADD COLUMN existing_column_name SET DATA TYPE

    NEW_DATA_TYPE

    ALTER TABLE table_name

        DROP COLUMN existing_column_name


    DROP TABLE table_name

    TRUNCATE TABLE table_name

        IMMEDIATE;

```

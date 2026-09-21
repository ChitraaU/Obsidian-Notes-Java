**Java Database Connectivity**
This is a Java API through which we can set up the connection with the database and interact with the database

Java Application -> JDBC-> MySql
You can use JDBC to:

- Connect to a database
- Execute SQL statements
- Retrieve results
- Insert/update/delete data
- Handle transactions
- Close database resources

**Maven Dependency : MySql Connector**

***Driver Manager***
This is a JDBC class which manages the database drivers and help us in connecting with the database
Connection connection = DriverManager.getConnection(URL,USER,PASSWORD);

***Try with Resources*** 

This is  a part of JDBC that closes the connection automatically it is a class of JDBC without it we have to use the finally block with the try catch resources once the work is done and we want to close the connection

## The JDBC flow you should remember

For now, think of JDBC like this:

```
1. Add MySQL Connector/J
          ↓
2. Create database URL
          ↓
3. DriverManager.getConnection()
          ↓
4. Get Connection
          ↓
5. Execute SQL
          ↓
6. Process ResultSet
          ↓
7. Resources automatically close
```


**Statement**
`Statement` is a **JDBC interface used to send SQL statements from your Java application to the database**.

The flow is:

```
Java Application
      ↓
Connection
      ↓
Statement
      ↓
SQL query
      ↓
Database
```

### What can `Statement` do?

Common methods include:

|Method|Purpose|
|---|---|
|`executeQuery()`|Executes a SELECT query|
|`executeUpdate()`|Executes INSERT, UPDATE, DELETE|
|`execute()`|Executes a general SQL statement|
**ResultSet**

`ResultSet` represents the **rows returned by a SELECT query**.
`rs.next()` moves to the next row.
# How Statement and ResultSet work together

The typical JDBC SELECT flow is:

```
Connection
    ↓
Statement
    ↓
executeQuery(SQL)
    ↓
ResultSet
    ↓
rs.next()
    ↓
read columns
```
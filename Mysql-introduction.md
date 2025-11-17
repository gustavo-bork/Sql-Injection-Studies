## Structured Query Language (SQL)

- Retrieve data
- Update data
- Delete data
- Create new tables and databases
- Add / Remove users
- Assign permissions to these users

## Command line

### Authenticate to MySQL database
```bash
mysql -u root -p
```

### Authenticate specifying host (-h) and port (-P)
```bash
mysql -u root -h docker.hackthebox.eu -P 3306 -p
```

### Create a database
```bash
mysql> CREATE DATABASE users;

Query OK, 1 row affected (0.02 sec)
```

### Show database
```bash
mysql> SHOW DATABASES;

+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
| users              |
+--------------------+

mysql> USE users;

Database changed
```

> [!TIP]
> SQL statements are case insensitive. However, the database name is case sensitive.

## Tables

### Create table statement
```sql
CREATE TABLE logins (
    id INT,
    username VARCHAR(100),
    password VARCHAR(100),
    date_of_joining DATETIME
);
```

### Show all tables in a database
```bash
mysql> USE <database>;
mysql> SHOW TABLES;
```

### Describe the details of a selected table
```bash
mysql> DESCRIBE <table name>;
```

### Table properties
```sql
  id INT NOT NULL AUTO_INCREMENT,
  username VARCHAR(100) UNIQUE NOT NULL,
  date_of_joining DATETIME DEFAULT NOW(),
  PRIMARY KEY (id)
```

- **AUTO_INCREMENT**: Increments automatically the selected column by one every time a new item is added.
- **NOT NULL**: Ensures a column is never left empty.
- **UNIQUE**: Ensures the column is never repeated.
- **DEFAULT**: Specifies the default value of a data type.

## SQL Statements

### INSERT Statement

```sql
INSERT INTO table_name VALUES (column1_value, column2_value, column3_value, ...);

-- Specify the column names to insert
INSERT INTO table_name(column2, column3, ...) VALUES (column2_value, column3_value, ...);
```

> [!TIP]
> Note: skipping columns with the 'NOT NULL' constraint will result in an error, as it is a required value.

### SELECT Statement

```sql
SELECT * FROM table_name;
SELECT column1, column2 FROM table_name; -- Query only the selected columns
```

### DROP Statement

```sql
DROP TABLE table_name;
```

> [!TIP]
> The 'DROP' statement will permanently and completely delete the table with no confirmation, so it should be used with caution.

### ALTER Statement
```sql
ALTER TABLE table_name ADD newColumn datatype; -- Add new column and set datatype
ALTER TABLE table_name RENAME COLUMN column to newColumn; -- Rename column
ALTER TABLE table_name MODIFY column newDatatype; -- Modify column's datatype
ALTER TABLE table_name DROP column_name;
```

### UPDATE Statement

```sql
UPDATE table_name SET column1=newvalue1, column2=newvalue2, ... WHERE <condition>;
```

> [!TIP]
> Note: we have to specify the 'WHERE' clause with UPDATE, in order to specify which records get updated. The 'WHERE' clause will be discussed next.
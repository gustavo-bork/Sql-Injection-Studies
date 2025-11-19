## Query results

### Sorting Results

```sql
SELECT * FROM table_name ORDER BY column;

-- Sort in descending order (default is ascending)
SELECT * FROM table_name ORDER BY column DESC; 

-- Sort by multiple columns
SELECT * FROM table_name ORDER BY column1 DESC, column2 ASC;
```

### Limit results

```sql
SELECT * FROM table_name LIMIT 2;

-- Limit with offset
SELECT * FROM table_name LIMIT 1, 2;
```

> [!TIP]
> Note: the offset marks the order of the first record to be included, starting from 0. For the above, it starts and includes the 2nd record, and returns two values.

### WHERE Clause

```sql
SELECT * FROM table_name WHERE <condition>;
```

> [!TIP]
> Note: String and date data types should be surrounded by single quote (') or double quotes ("), while numbers can be used directly.

### LIKE Clause

```sql
-- % is a wildcard that matches all characters after string
SELECT * FROM table_name WHERE column LIKE 'string%';

-- % matches all characters before string
SELECT * FROM table_name WHERE column LIKE '%string';

-- % matches all characters before and after string
SELECT * FROM table_name WHERE column LIKE '%string%';
```

```sql
-- _ is used to match exactly one character
SELECT * FROM table_name WHERE column LIKE '_';
```
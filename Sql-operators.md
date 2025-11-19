## SQL Operators

### AND Operator
```sql
SELECT * FROM table_name WHERE <condition1> AND <condition2>;
```

### OR Operator
```sql
SELECT * FROM table_name WHERE <condition1> OR <condition2>;
```

### NOT Operator
```sql
SELECT * FROM table_name NOT <condition>;
```

### Symbol Operators

- The `AND`, `OR` and `NOT` operators can also be represented as `&&`, `||` and `!`, respectively.

### Multiple Operator Precedence

- Determines the order of the operations
- List of common operations and their preference:
    1. Division (`/`), Multiplication (`*`) and Modulus (`%`)
    2. Addition (`+`) and subtraction (`-`)
    3. Comparison (`=`, `>`, `<`, `<=`, `>=`, `!=`, `LIKE`)
    4. NOT (`!`)
    5. AND (`&&`)
    6. OR (`||`)
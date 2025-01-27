# NULL Values

- Null represents a missing or unknown value
- In real world database can have empty values because of human errors or because information not available

# IS NULL

```sql
SELECT name
FROM people
WHERE birth_date IS NULL;
```

# IS NOT NULL

```sql
SELECT COUNT(name) AS count_birth_date
FROM people
WHERE birth_date IS NOT NULL;
```

# COUNT AND NOT NULL

- COUNT() vs IS NOT NULL
  There may be a question about the difference between using COUNT with a field name and using the same COUNT with the added WHERE clause with IS NOT NULL. The answer is there is no difference, as both will be counting non-missing values.

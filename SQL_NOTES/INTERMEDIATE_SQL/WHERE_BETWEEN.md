## FILTER

- To filter we need to use **WHERE**
- example To filter films except which released in 1960

```sql
SELECT
    title
FROM films
WHERE release_year <> 1960;
```

## Written order of WHERE

- SELECT FROM WHERE LIMIT

## ORDER OF EXECUTION WITH WHERE

- FROM WHERE SELECT LIMIT

**We can add multiple criteria in WHERE clause by using OR ,AND , BETWEEN**

**BETWEEN is inclusive**

```SQL
SELECT * FROM Products
WHERE Price BETWEEN 10 AND 20;
```

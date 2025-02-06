## UNION INTERSECT AND EXCEPT

- UNION INTERSECT AND EXCEPT are the SET operators
  # prerequisites to do union
  1. Both SELECT statements should contain same number of columns
  2. Columns should have same data types

## UNION

- The SQL UNION operator is used to combine the result sets of two or more SELECT queries into a single result set.
- **Every select statement within union must have same columns**

- In **BigQuery** cannot write union without a qualifier which is **ALL or DISTINCT**
- **ALL** : you will get all of the rows in first table and all of rows in second table regardless of duplicates.
- Common rows are kept
- **DISTINCT** : you will get unique rows in first and second table
- common rows are discarded in DISTINCT
- Union comes from Mathematical SET terminology

```sql
SELECT * FROM fantasy.toy1

UNION DISTINCT

SELECT * FROM fantasy.toy2
```

## INTERSECT

- If you only want rows between two select statements which are common then we use intersect

```sql
SELECT * FROM fantasy.toy1

INTERSECT DISTINCT

SELECT * FROM fantasy.toy2
```

# Give me everything from toy 1 except the rows shared with toy 2

```sql
SELECT * FROM fantasy.toy1

EXCEPT DISTINCT

SELECT * FROM fantasy.toy2
```

- **EXCEPT** is not symmetrical

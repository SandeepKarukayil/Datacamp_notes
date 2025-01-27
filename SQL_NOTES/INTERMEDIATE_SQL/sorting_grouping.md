## GROUPING

- If we want to group our data based on fields we use GROUP BY

## GROUP BY single fields

```sql
SELECT certification ,
COUNT(title) AS title_count
FROM films
GROUP BY certification

```

- SQL will try to return an error if we try to select a field that is not in our GROUP BY clause to correct this we need to use aggregate function around title

## GROUP BY WITH ORDER BY

```sql
SELECT certification ,
COUNT(title) AS title_count
FROM films
GROUP BY certification
ORDER BY title_count DESC;
```

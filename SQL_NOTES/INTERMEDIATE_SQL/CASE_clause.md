## CASE

- CASE clause allows user to apply conditional logic in sql
- It is useful for bucketing data or classifying data to get a broader picture of the data
- CASE clause has keywords CASE and END and within the WHEN and THEN is used to use conditional logic
- **CASE** clause will keep on executing unless it gets true or all case clauses ends
- **ELSE** clause takes care of all the conditions which we didn't specify
- You cannot mix types in case clauses like using data type for condition 1 and another data type for condition 2
- if no condition satisfy it will output that record as **NULL**
- In order of execution **CASE** clause executes at SELECT statement

```sql
-- level < 15 low
-- level between 15 and 25 mid
-- level above 25 super
SELECT name,level,level>=20 AS level_at_least_20,
CASE
  WHEN level<15 THEN "low"
  WHEN level>=15 AND level<25 THEN "mid"
  WHEN level>=25  THEN "super"
  ELSE "GOD"
END AS level_bucket
FROM fantasy.characters
WHERE is_alive = true
```

- If you don't use coma after select statement before CASE you will get error

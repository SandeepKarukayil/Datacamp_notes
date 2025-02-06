## SORTING DATA

- Sorting means we want to put our data in a specific order.

# ORDER BY

- IN SQL ORDER BY keyword is used to sort the results of one or more fields.
- By default ORDER BY will sort in Ascending order(small to big or A to Z).
- Symbols and numbers come before A
- null is highest value and comes before number
- ASC : Ascending order
- DESC : Descending order

```sql
SELECT title, budget
FROM films
ORDER BY budget ASC;
```

-ORDER BY MULTIPLE FIELDS

- ORDER BY field1,field2,field3,...
- Field 2 is like a tie breaker when field1 is not decisive it sorts using field2

# Order of execution

ORDER BY falls towards the end of the order of execution we already know, coming in just before limit. The FROM statement will execute first, then WHERE, followed by SELECT, ORDER BY, and finally, LIMIT.

## Filter text

- Filter a pattern rather than a specific text
- We use LIKE , NOT LIKE , IN

## LIKE

- Used to search for a pattern in a field
- We use two wild cards with like
- 1. % : will match zero , 1 or many characters in a text

  ```sql
  SELECT name
  FROM people
  WHERE name LIKE 'Ade%';
  ```

  RESULT : Adel karam , Adelaide , Aden young

- 2. \_ : underscore wildcard will match a single character in a text

```sql
    SELECT name
    FROM people
    WHERE name LIKE 'Ev_'
```

RESULT : Eve

-NOT LIKE : gets the data which dont match the pattern.

- This operation is case sensitive

## WHERE IN

- If we want to search for text with multiple query and there is OR chain we can use IN
- ```sql
    SELECT title
    FROM films
    WHERE release_year IN (1920,1930,1940);
  ```

## Sumarizing using aggregate function

# Sumarizing means to get a brief idea of database

- The aggregate functions which help us to summarize are

1. COUNT() : can be used on NUMERIC AS WELL AS NON NUMERIC
2. AVG() : NUMERIC FIELDS ONLY
3. SUM() : NUMERIC FIELDS ONLY
4. MIN() : can be used on NUMERIC AS WELL AS NON NUMERIC
5. MAX() : can be used on NUMERIC AS WELL AS NON NUMERIC

- **We operate on fields or columns with aggregate functions and not on RECORDS OR ROWS**

- **Best practice to using ALIAS when summarizing data**

# ROUND

- it is used to round the decimal numbers.
- it has two parameters first is the number , second is the number of decimal places we need to round.
- If we want to round to whole number skip the second parameter
- It can also take negative numbers and it will select left of decimal
- ROUND CAN ONLY BE USED WITH NUMERIC FIELDS

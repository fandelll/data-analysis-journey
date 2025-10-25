Date: 10/24/2025
1. The INNER JOIN (matches rows from the first table and the second table which have the same key (as defined by the ON constraint) to create a result row with the combined columns from both tables.)
   ONLY keep matched value
2. LEFT/RIGHT/FULL JOIN
   LEFT JOIN (Based on the left table, simply includes rows from A regardless of whether a matching row is found in B, if not found, shown as NULL)
   RIGHT JOIN (Based on the right table,  keeping rows in B regardless of whether a match is found in A)
   FULL JOIN (simply means that rows from both tables are kept, regardless of whether a matching row exists in the other table.)
   Exercise 7: Question 1
   Sometimes the app doesn't have a FULL JOIN
3. IS/IS NOT NULL
4. COUNT(*), COUNT(column)
5. MIN(column)
6. MAX(column)
7. AVG(column)
8. SUM(column)
9. GROUP BY
10. HAVING group_condition;
11. SELECT DISTINCT column, AGG_FUNC(column_or_expression), …
FROM mytable
    JOIN another_table
      ON mytable.column = another_table.column
    WHERE constraint_expression
    GROUP BY column
    HAVING constraint_expression
    ORDER BY column ASC/DESC
    LIMIT count OFFSET COUNT;
    Exercise 12

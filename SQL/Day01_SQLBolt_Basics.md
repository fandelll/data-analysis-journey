date: 10/22/2025
SQl day1------
condition: 
=, !=, <, <=, >, >=
BETWEEN ... AND ... (inclusive) e.g. col_name BETWEEN 1.5 AND 10.5
NOT BETWEEN ... AND ... (inclusive) e.g. col_name NOT BETWEEN 1 AND 10
IN(...) e.g. col_name IN (2, 4, 6)
NOT IN(...) e.g. col_name NOT IN (1, 3, 5)
FOR STRING:
= e.g. col_name = "abc"
!=, <, > e.g.col_name != "abcd"
LIKE, e.g. col_name LIKE "ABC"
NOT LIKE, e.g. 	col_name NOT LIKE "ABCD"
% e.g. col_name LIKE "%AT%" (matches "AT", "ATTIC", "CAT" or even "BATS")
_ e.g. col_name LIKE "AN_" (matches "AND", but not "AN")
IN (...) e.g. col_name IN ("A", "B", "C")
NOT IN(...) e.g. col_name NOT IN ("D", "E", "F");
DISTINCT;
ORDER BY ... ASC/DESC;
LIMIT num_limit OFFSET num_offset; The LIMIT will reduce the number of rows to return, and the optional OFFSET will specify where to begin counting the number rows from. （LIMIT 2 OFFSET 2 代表3，4）

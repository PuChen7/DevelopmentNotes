# Content
- [UNION, INTERSECT, and EXCEPT](#-UNION,-INTERSECT,-and-EXCEPT)
- [GROUP BY and HAVING](#GROUP-BY-and-HAVING)

## UNION, INTERSECT, and EXCEPT
`UNION`, `INTERSECT`, and `EXCEPT` can be used on any two tables that are **union-compatible**, that is, have the same number of columns and the columns, taken in order, have the same types.

## GROUP BY and HAVING
```sql
SELECT [ DISTINCT ] select-list
FROM from-list
WHERE qualification
GROUP BY grouping-list
HAVING group-qualification
```

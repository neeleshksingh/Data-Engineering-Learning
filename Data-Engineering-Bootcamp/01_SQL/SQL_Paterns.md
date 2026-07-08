| Pattern                    | Think                          |
| -------------------------- | ------------------------------ |
| For each...                | GROUP BY                       |
| Need another table         | JOIN                           |
| Keep all rows + extra info | Window Function                |
| Previous row               | LAG                            |
| Next row                   | LEAD                           |
| Top N                      | ROW_NUMBER / RANK / DENSE_RANK |


| If the question says...         | Think...                                 |
| ------------------------------- | ---------------------------------------- |
| For each department             | `GROUP BY`                               |
| Compare with department average | Window Function                          |
| Compare with previous row       | `LAG()`                                  |
| Compare with next row           | `LEAD()`                                 |
| Rank inside each department     | `ROW_NUMBER()`, `RANK()`, `DENSE_RANK()` |


| Pattern                       | Think                                  |
| ----------------------------- | -------------------------------------- |
| Need one value for each group | Aggregate (`SUM`, `AVG`, `MAX`, `MIN`) |
| Need calculation on each row  | Arithmetic (`+`, `-`, `*`, `/`)        |


## Window Functions

### When to use?

- Need to keep all rows.
- Need extra information for each row.
- Compare with group average.
- Compare with group maximum.
- Compare with previous/next row.
- Ranking.

### Mental Checklist

1. One table?
2. Need all rows?
3. Need extra information?
4. Window Function.

| Pattern        | Example                     |
| -------------- | --------------------------- |
| Aggregation    | Revenue by month            |
| Ranking        | Top 3 salaries              |
| Comparison     | Salary > department average |
| Previous/Next  | Consecutive logins          |
| Existence      | Customers who never ordered |
| Dates          | Day 1 retention             |
| Running totals | Cumulative sales            |
| Top N          | Highest paid employees      |
| Gaps & Islands | Consecutive dates           |
| Pivot          | Monthly report              |

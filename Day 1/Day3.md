# Day 3
## Problem 1: Find the Top 3 Employees by Salary in Each Department

### Objective
Given a table of employees with their respective departments and salaries, find the top 3 employees with the highest salaries in each department.

### Input Table - `employees`:

| emp_id | emp_name | department | salary |
|--------|----------|------------|--------|
| 1      | Alice    | HR         | 80000  |
| 2      | Bob      | IT         | 120000 |
| 3      | Carol    | HR         | 85000  |
| 4      | Dave     | IT         | 90000  |
| 5      | Eve      | HR         | 95000  |
| 6      | Frank    | IT         | 110000 |
| 7      | Grace    | IT         | 115000 |

### Output:
The output should list the top 3 employees by salary in each department.

| emp_id | emp_name | department | salary |
|--------|----------|------------|--------|
| 5      | Eve      | HR         | 95000  |
| 3      | Carol    | HR         | 85000  |
| 1      | Alice    | HR         | 80000  |
| 2      | Bob      | IT         | 120000 |
| 7      | Grace    | IT         | 115000 |
| 6      | Frank    | IT         | 110000 |

### Constraints
- Assume each department has at least three employees.
- Salaries are positive integers.

### Example
#### Input:
```plaintext
emp_id | emp_name | department | salary
----------------------------------------
1      | Alice    | HR         | 80000
2      | Bob      | IT         | 120000
3      | Carol    | HR         | 85000
4      | Dave     | IT         | 90000
5      | Eve      | HR         | 95000
6      | Frank    | IT         | 110000
7      | Grace    | IT         | 115000
```

#### Output:
```plaintext
emp_id | emp_name | department | salary
----------------------------------------
5      | Eve      | HR         | 95000
3      | Carol    | HR         | 85000
1      | Alice    | HR         | 80000
2      | Bob      | IT         | 120000
7      | Grace    | IT         | 115000
6      | Frank    | IT         | 110000
```

### Instructions
- Write a query to retrieve the top 3 employees by salary from each department.
- Consider ties in salaries; if multiple employees have the same salary within the top 3, include all of them.

---

This problem requires basic SQL querying knowledge to filter and sort data based on grouped conditions.


Here’s a problem statement based on the image you provided:

```markdown
## Problem 2: Find Products Sold on the Last Day of Each Month

### Objective
Given a table of sales data with product names and sale dates, identify all the products that were sold on the last day of each month.

### Input Table - `sales`:

| sale_id | product_name | sale_date |
|---------|--------------|-----------|
| 1       | Laptop       | 2024-01-31|
| 2       | Mouse        | 2024-01-25|
| 3       | Keyboard     | 2024-02-28|
| 4       | Monitor      | 2024-02-28|
| 5       | Laptop       | 2024-03-31|

### Output:
The output should list the `sale_id`, `product_name`, and `sale_date` for the products sold on the last day of each month.

### Constraints
- The `sale_date` is in `YYYY-MM-DD` format.
- A month can have multiple products sold on the last day.

### Example
#### Input:
```plaintext
sale_id | product_name | sale_date
-----------------------------------
1       | Laptop       | 2024-01-31
2       | Mouse        | 2024-01-25
3       | Keyboard     | 2024-02-28
4       | Monitor      | 2024-02-28
5       | Laptop       | 2024-03-31
```

#### Output:
```plaintext
sale_id | product_name | sale_date
-----------------------------------
1       | Laptop       | 2024-01-31
3       | Keyboard     | 2024-02-28
4       | Monitor      | 2024-02-28
5       | Laptop       | 2024-03-31
```

### Instructions
- Write a query to retrieve the sales records of products sold on the last day of each month.
- Ensure that the query correctly handles months with different numbers of days (e.g., February).

---

This problem requires knowledge of SQL date functions to identify the last day of each month and filter records accordingly.
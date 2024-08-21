Here’s the revised `problem.md` file with the examples removed:

```markdown
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

### Output
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

### Instructions
- Write a query to retrieve the top 3 employees by salary from each department.
- Consider ties in salaries; if multiple employees have the same salary within the top 3, include all of them.

---

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

### Output
The output should list the `sale_id`, `product_name`, and `sale_date` for the products sold on the last day of each month.

### Constraints
- The `sale_date` is in `YYYY-MM-DD` format.
- A month can have multiple products sold on the last day.

### Instructions
- Write a query to retrieve the sales records of products sold on the last day of each month.
- Ensure that the query correctly handles months with different numbers of days (e.g., February).

---

## Problem 3: Find the Second Highest Salary Without Using `LIMIT` or `TOP`

### Input Table - `employees`:

| emp_id | emp_name | salary  |
|--------|----------|---------|
| 1      | Alice    | 80000   |
| 2      | Bob      | 120000  |
| 3      | Carol    | 85000   |
| 4      | Dave     | 90000   |
| 5      | Eve      | 95000   |

### Problem Description
You are given a table named `employees`, where each row contains details about an employee's ID, name, and salary. The task is to write a SQL query to find the second highest salary from the table without using the `LIMIT` or `TOP` clause.

### Expected Output
The second highest salary from the `employees` table:

| salary  |
|---------|
| 95000   |

---

## Problem 4: Find Employees Who Have the Same Salary as Someone in Another Department

### Input Table - `employees`:

| emp_id | emp_name | department | salary  |
|--------|----------|------------|---------|
| 1      | Alice    | HR         | 80000   |
| 2      | Bob      | IT         | 120000  |
| 3      | Carol    | HR         | 95000   |
| 4      | Dave     | IT         | 90000   |
| 5      | Eve      | Sales      | 95000   |

### Problem Description
You are given a table named `employees`, which contains employee details including their ID, name, department, and salary. The task is to write a SQL query to find all employees who have the same salary as someone in a different department.

### Expected Output
The employees who have the same salary as someone in a different department:

| emp_name |
|----------|
| Carol    |
| Eve      |

---

## Problem 5: Find All Employees Who Don’t Have a Manager

### Input Tables - `employees`, `managers`:

#### Table `employees`:

| emp_id | emp_name | manager_id |
|--------|----------|------------|
| 1      | Alice    | 2          |
| 2      | Bob      | NULL       |
| 3      | Carol    | 1          |
| 4      | Dave     | 2          |
| 5      | Eve      | 1          |

### Problem Description
You are given a table named `employees`, which contains information about employees, including their IDs, names, and the ID of their manager. The task is to write a SQL query to find all employees who do not have a manager (i.e., their `manager_id` is `NULL`).

### Expected Output:
The output of the query would be:
```plaintext
emp_name
---------
Bob

---

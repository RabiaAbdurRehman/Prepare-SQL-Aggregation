--Problem

We define an employee's total earnings to be their monthly salary * months  worked, and the maximum total 
earnings to be the maximum total earnings for any employee in the Employee table. Write a query to find the 
maximum total earnings for all employees as well as the total number of employees who have maximum total
earnings. Then print these values as 2 space-separated integers.

The Employee table containing employee data for a company is described as follows:
+-------------+------------+
| Column       |   Type     |
+-------------+------------+
| employee_id | INTEGER    |
| name        | String     |
| months      | INTEGER    |
| salary      | INTEGER    |
+-------------+------------+

--Solution

SELECT salary * months AS maxSalary, 
COUNT(*) FROM EMPLOYEE
GROUP BY maxSalary 
ORDER BY maxSalary DESC
LIMIT 1;

--Expected Output
108064 7

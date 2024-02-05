--Problem

Samantha was tasked with calculating the average monthly salaries for all employees in the EMPLOYEES table, but did not realize her keyboard's 0 key was broken until after completing the calculation. 
She wants your help finding the difference between her miscalculation(using salaries with any zeros removed), and the actual average salary.

The EMPLOYEES table is described as follows:

+-------------+------------+
|Column       |   Type     |
+-------------+------------+
| ID          | INTEGER    |
| Name        | STRING     |
|  Salary     | INTEGER    |
+-------------+------------+

--Solution
SELECT CEIL(AVG(Salary) - AVG(REPLACE(Salary,"0", "")))
FROM EMPLOYEES;

--Explanation
CEIL(AVG(...)) calculates the average after removing zeros and rounds it up to the next integer.
REPLACE(Salary, '0', '') removes any occurrences of the digit '0' from the "Salary" column.

--Problem
Query the following two values from the STATION table:

.The sum of all values in LAT_N rounded to a scale of 2 decimal places.
.The sum of all values in LONG_W rounded to a scale of 2  decimal places.

The STATION table is described as follows:
+-------------+------------+
| Field       |   Type     |
+-------------+------------+
| ID          | INTEGER    |
| CITY        | VARCHAR(21)|
| STATE       | VARCHAR(2) |
| LAT_N       | NUMERIC    |
| LONG_W      | NUMERIC    |
+-------------+------------+

--Solution
SELECT ROUND(SUM(LAT_N), 2), ROUND(SUM(LONG_W), 2) FROM STATION;

--Expected Output
42850.04 47381.48

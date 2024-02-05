--Problem
Query the average population for all cities CITY, rounded down to the nearest integer.
Given a City table, whose fields are described as

+-------------+----------+
| Field       | Type     |
+-------------+----------+
| ID          | int(11)  |
| Name        | char(35) |
| CountryCode | char(3)  |
| District    | char(20) |
| Population  | int(11)  |
+-------------+----------+

--Solution

SELECT ROUND(AVG(POPULATION))FROM CITY;

--Expected Output
454250

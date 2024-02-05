--Problem

Query the difference between the maximum and minimum populations in CITY.
The CITY table is described as follows:

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

SELECT MAX(POPULATION)- MIN(POPULATION) AS DIFFERENCEPOP FROM CITY;

--Expected Output
4695354

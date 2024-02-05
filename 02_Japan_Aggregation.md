--Problem

Query the sum of populations for all Japansese cities in CITY. The COUNTRYCODE for Japan is JPN.
The CITY table is descirbed as follows


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

SELECT SUM(POPULATION) FROM CITY
WHERE COUNTRYCODE = "JPN";

--Expected Output
879196

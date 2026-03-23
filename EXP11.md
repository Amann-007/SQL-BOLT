# EXPERIMENT-11
# 01. Find the number of Artists in the studio (without a HAVING clause)
 Query
~~~sql   
SELECT role, COUNT(*) as Number_of_artists
FROM employees
WHERE role = "Artist";
~~~
# 02. Find the number of Employees of each role in the studio 
 Query
~~~sql   
SELECT role, COUNT(*)
FROM employees
GROUP BY role;
~~~
# 03.Find the total number of years employed by all Engineers
 Query
~~~sql   
SELECT role, SUM(years_employed)
FROM employees
GROUP BY role
HAVING role = "Engineer";
~~~


# EXPERIMENT-10
# 01. Find the longest time that an employee has been at the studio
 Query
~~~sql   
SELECT Name,Years_employed FROM employees
ORDER BY Years_employed DESC 
Limit 1;
~~~
# 02. For each role, find the average number of years employed by employees in that role
 Query
~~~sql   
SELECT role, AVG(years_employed) as Average_years_employed
FROM employees
GROUP BY role;
~~~
# 03.Find the total number of employee years worked in each building 
 Query
~~~sql   
SELECT building, SUM(years_employed) as Total_years_employed
FROM employees
GROUP BY building;
~~~

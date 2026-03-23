# EXPERIMENT-7
# 01. Find the list of all buildings that have employees
 Query
~~~sql   
SELECT DISTINCT Buildings.Building_name 
FROM Buildings INNER JOIN Employees  
ON Buildings.Building_name= Employees.Building;
~~~
# 02.Find the list of all buildings and their capacity  
 Query
~~~sql   
SELECT DISTINCT Building_name,Capacity
FROM Buildings ;
~~~
# 03. List all buildings and the distinct employee roles in each building (including empty buildings)
 Query
~~~sql   
SELECT DISTINCT buildings.building_name, employees.role
FROM buildings LEFT JOIN employees
ON buildings.building_name = employees.building;
~~~

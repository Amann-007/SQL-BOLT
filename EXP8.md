# EXPERIMENT-8
# 01. Find the name and role of all employees who have not been assigned to a building 
 Query
~~~sql   
SELECT Name,Role
FROM Employees 
WHERE Building is NULL;
~~~
# 02.Find the names of the buildings that hold no employees  
 Query
~~~sql   
SELECT buildings.building_name
FROM buildings
LEFT JOIN employees
ON buildings.building_name = employees.building
WHERE employees.building IS NULL;
~~~

# EXPERIMENT-1
# 01. Find the movie with a row id of 6  
 Query
~~~sql   
SELECT * FROM movies
where Id=6;
~~~
# 02. Find the movies released in the years between 2000 and 2010  
 Query
~~~sql   
SELECT * FROM movies
where Year BETWEEN 2000 AND 2010;
~~~
# 03. Find the movies not released in the years between 2000 and 2010  
 Query
~~~sql   
SELECT * FROM movies
where Year NOT BETWEEN 2000 AND 2010;
~~~
# 04. Find the first 5 Pixar movies and their release year 
 Query
~~~sql   
SELECT * FROM movies
LIMIT 5;
~~~
# EXPERIMENT-3
# 01. Find all the Toy Story movies
 Query
~~~sql   
SELECT * FROM movies
WHERE Title like "Toy Story%";
~~~
# 02. Find all the movies directed by John Lasseter 
 Query
~~~sql   
SELECT * FROM movies
WHERE Director = "John Lasseter";
~~~
# 03.Find all the movies (and director) not directed by John Lasseter  
 Query
~~~sql   
SELECT * FROM movies
WHERE Director != "John Lasseter";
~~~
# 04. Find all the WALL-* movies
 Query
~~~sql   
SELECT * FROM movies
WHERE Title like "WALL%";
~~~

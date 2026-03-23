# EXPERIMENT-9
# 01. List all movies and their combined sales in millions of dollars
 Query
~~~sql   
SELECT Title,
(Boxoffice.Domestic_sales+Boxoffice.International_sales)/1000000 AS Total_sales
FROM Movies INNER JOIN Boxoffice 
ON movies.id = boxoffice.movie_id;
~~~
# 02. List all movies and their ratings in percent
 Query
~~~sql   
SELECT Title,Boxoffice.Rating*10 AS Rating_percent
FROM Movies INNER JOIN Boxoffice 
ON movies.id = boxoffice.movie_id;
~~~
# 03. List all movies that were released on even number years
 Query
~~~sql   
SELECT Title,Year
FROM Movies
WHERE Year%2==0 ;
~~~

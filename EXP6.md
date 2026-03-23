# EXPERIMENT-6
# 01.Find the domestic and international sales for each movie  
 Query
~~~sql   
SELECT Title,Domestic_sales,International_sales 
FROM Movies INNER JOIN Boxoffice 
ON movies.id = boxoffice.movie_id;

~~~
# 02. Show the sales numbers for each movie that did better internationally rather than domestically
 Query
~~~sql   
SELECT Title,Domestic_sales,International_sales 
FROM Movies INNER JOIN Boxoffice 
ON movies.id = boxoffice.movie_id
WHERE Domestic_sales < International_sales; 
~~~
# 03. List all the movies by their ratings in descending order
 Query
~~~sql   
SELECT Title,Domestic_sales,International_sales 
FROM Movies INNER JOIN Boxoffice 
ON movies.id = boxoffice.movie_id
ORDER BY Rating DESC;
~~~

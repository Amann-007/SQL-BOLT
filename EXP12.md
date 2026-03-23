# EXPERIMENT-12
# 01. Find the number of movies each director has directed
 Query
~~~sql   
SELECT director, COUNT(id) as Num_movies_directed
FROM movies
GROUP BY director;
~~~
# 02. Find the total domestic and international sales that can be attributed to each director
 Query
~~~sql   
SELECT director, SUM(domestic_sales + international_sales) as Cumulative_sales_from_all_movies
FROM movies
    INNER JOIN boxoffice
        ON movies.id = boxoffice.movie_id
GROUP BY director;
~~~

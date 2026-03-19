# EXPERIMENT-4
# 01.List all directors of Pixar movies (alphabetically), without duplicates
```sql
SELECT DISTINCT director
FROM movies
ORDER BY director;
```

# 02.List the last four Pixar movies released (ordered from most recent to least)
```sql
SELECT title
FROM movies
ORDER BY year DESC
LIMIT 4;
```

# 03.List the first five Pixar movies sorted alphabetically
```sql
SELECT title
FROM movies
ORDER BY title ASC
LIMIT 5;
```

# 04.List the next five Pixar movies sorted alphabetically
```sql
SELECT title
FROM movies
ORDER BY title ASC
LIMIT 5 OFFSET 5;
```
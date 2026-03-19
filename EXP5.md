# EXPERIMENT-5
# 01.List all the Canadian cities and their populations
```sql
SELECT city, population
FROM north_american_cities
WHERE country = 'Canada';
```

# 02.Order all the cities in the United States by their latitude from north to south
```sql
SELECT city, population
FROM north_american_cities
WHERE country = 'Canada';
```

# 03.List all the cities west of Chicago, ordered from west to east
```sql
SELECT city
FROM north_american_cities
WHERE longitude < -87.6298
ORDER BY longitude ASC;
```

# 04.List the two largest cities in Mexico (by population)
```sql
SELECT city
FROM north_american_cities
WHERE country = 'Mexico'
ORDER BY population DESC
LIMIT 2;
```

# 05.List the third and fourth largest cities (by population) in the United States and their population
```sql
SELECT city, population
FROM north_american_cities
WHERE country = 'United States'
ORDER BY population DESC
LIMIT 2 OFFSET 2;
```
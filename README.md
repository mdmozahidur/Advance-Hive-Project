# Advance-Hive-Project

Dataset - action, thriller, comedy, animation and action_comedy_thriller_animation

a) Write a hive query to select last 50 distinct records from *table* after sorting it by
movie_name in descending order
b) Write a hive query to select to 10 distinct records from *table* after distributing it by genre
c) Write a hive query to count movies released by years from *table*
d) Write a hive query to find all animation movies released after year 2000 from *table*
e) Select t.year, count(t.year) as count from (Select regexp_extract(movie_name, '(\\d{4})',1)
as year from *table* where genre='Animation') t group by year order by count desc limit 10;
f) Select t.year, count(t.year) as count from (Select regexp_extract(movie_name, '(\\d{4})',1)
as year from *table* where genre='Comedy') t group by year order by count desc limit 20;
g) Extract movie released year from the movie title and store it by creating an additional
attribute in a new table

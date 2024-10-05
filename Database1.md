# Week 3
## Exercise 2 - Single table queries
### Question 1
select * from goal;
![screenshot](screenshot1.png)

### Question 2
select name,type from airport where iso_country ='Fi';
![screenshot](Screenshot2.png)

### Question 3
select name from airport where iso_country = 'Fi' order by name Asc;
![screenshot](Screenshot3.png)

### Question 4
select name,type from airport where iso_country = 'Fi' order by type,name;
![screenshot](Screenshot4.png)

### Question 5
select name from country where name like 'F%';
![screenshot](Screenshot5.png)

### Question 6
select name from country where name like '%F%';
![screenshot](Screenshot6.png)

### Question 7
select location from game where screen_name = "vesa";
![screenshot](Screenshot7.png)

### Question 8
select CO2_consumed from game where screen_name = "Ilkka";
![screenshot](Screenshot8.png)

### Question 9
select distinct CO2_budget from game;
![screenshot](Screenshot9.png)

### Question 10
SET @ CO2_left :=(SELECT SUM (CO2_budget-CO2_consumed)FROM game where screen_name ='Ilkka');
Select screen_name, CO2_budget,CO2_consumed,@CO2_left from game where screen_name = 'Ilkka';
![screenshot](Screenshot10.png)

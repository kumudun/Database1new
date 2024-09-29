# Week 3
## Exercise 1 - Single table queries
### Question 1
select * from goal;
![screenshot](Screenshot-Q 1.png)

### Question 2
select name,type from airport where iso_country ='Fi';
![screenshot](Screenshot-Q 2.png)

### Question 3
select name from airport where iso_country = 'Fi' order by name Asc;
![screenshot](Screenshot-Q 3.png)

### Question 4
select name,type from airport where iso_country = 'Fi' order by type,name;
![screenshot](Screenshot-Q 4.png)

### Question 5
select name from country where name like 'F%';
![screenshot](Screenshot-Q 5.png)

### Question 6
select name from country where name like '%F%';
![screenshot](Screenshot-Q 6.png)

### Question 7
select location from game where screen_name = "vesa";
![screenshot](Screenshot-Q 7.png)

### Question 8
select CO2_consumed from game where screen_name = "Ilkka";
![screenshot](Screenshot-Q 8.png)

### Question 9
select distinct CO2_budget from game;
![screenshot](Screenshot-Q 9.png)

### Question 10
set @ CO2_left:=(select sum(CO2_budget-CO2_consumed)from game where screen_name ='Ilkka');select screen_name,C
O2_budget,CO2_consumed,@CO2_left from game where screen_name = 'Ilkka';
![screenshot](Screenshot-Q 10.png)






 
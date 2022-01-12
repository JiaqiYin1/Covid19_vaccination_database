# Covid19_vaccination_database
Database: world_covid19_vaccination
Description:
Most countries in the world are vaccinating against COVID-19. These countries have unique names, country abbreviations, and the vaccine that they are using. Each vaccine has a name, a type (inactivated or mRNA vaccine...), R&D companies, protection rates. Countries are divided into many states/provinces. Each state has its name, the country where the state is located, and a different population. In the state, there are a lot of hospitals performing the tasks. Each hospital has its own name, the state where it is located, the city where the hospital is located, and vaccinated people. People who go to be vaccinated will have a unique number, and the hospital that she/he went to, ID, name, age, date of birth.


Part 2 – CRUD (Create, read, update, and delete)

List of strong entities:
1. vaccine

List of weak entities:
1. country
2. state 
3. hospital
4. people

We will implement the following functionality using Java and SQL with necessary GUI interfaces.
1. Insert/read/delete/update country table.
2. Insert/read/delete/update vaccine table.
3. Insert/read/delete/update people table (all attributes except the number). The number should be generated by the system automatically using MySQL autoincrement.
 



Part 3 – Queries 
Based on the Demo, we will implement the following functionality using Java and SQL with necessary GUI interfaces.
Trivial Queries:

1. List all information of people who got vaccines from the input hospital.
We used ‘where’

2. List all information of countries ordered by country abbreviation desc.
We used ‘order by’

3. List all vaccine types and their average protection rate.
We used ‘ave()’ and ‘group by’

Non-trivial Queries:

1. List all countries and their population.
We used sum(), join, group by, and order by

2. List all hospitals and the information of vaccines that they are using.
We joined 3 tables, and nested queries were used

3. List all states whose number of vaccinated people > 150,000.
We used sum(), join, group by, and having clause

4. List all states whose population is greater than the average population in its country, its country, and its population.
We included correlated nested query in this one

5. List all information of people whose age is greater than the average age of vaccinated people in the same hospital.
We used join and also included correlated nested query in this one

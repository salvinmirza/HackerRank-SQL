<h6>Revising the Select Query I</h6>
SELECT * FROM CITY
WHERE COUNTRYCODE = 'USA' AND POPULATION > 100000;

<br />

<h6>Revising the Select Query II</h6>
SELECT NAME FROM CITY 
WHERE COUNTRYCODE = 'USA' AND POPULATION > 120000;

<br />

<h6>Select All</h6>
SELECT * FROM CITY 

<br />

<h6>Select By ID</h6>
SELECT * FROM CITY 
WHERE ID = 1661;

<br />

<h6>Japanese Cities' Attributes</h6>
SELECT * FROM CITY
WHERE COUNTRYCODE = 'JPN';

<br />

<h6>Japanese Cities' Names</h6>
SELECT NAME FROM CITY
WHERE COUNTRYCODE = 'JPN';

<br />

<h6>Weather Observation Station 1</h6>
SELECT CITY, STATE FROM STATION

<br />
<h6>Weather Observation Station 3</h6>
SELECT DISTINCT CITY FROM STATION
WHERE ID%2=0;

<br />
<h6>Weather Observation Station 4</h6>
SELECT COUNT(CITY) - COUNT (DISTINCT CITY)
FROM STATION ;



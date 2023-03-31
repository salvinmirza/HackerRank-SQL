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

<br />
<h6>Weather Observation Station 5</h6>

SELECT CITY, LENGTH(CITY) FROM STATION
ORDER BY LENGTH(CITY), CITY
LIMIT 1;

SELECT CITY, LENGTH(CITY) FROM STATION
ORDER BY LENGTH(CITY) DESC, CITY
LIMIT 1;

<br />
<h6>Weather Observation Station 6</h6>
SELECT DISTINCT CITY FROM STATION
WHERE CITY REGEXP '^[aeiou]';

<br />
** Learning REGEXP **

https://www.youtube.com/watch?v=KoltE-JUY0c&ab_channel=golearnfast

<br />
<h6>Weather Observation Station 7</h6>
SELECT DISTINCT CITY FROM STATION
WHERE CITY REGEXP '[aeiou]$';

<br />
<h6>Weather Observation Station 8</h6>
SELECT DISTINCT CITY FROM STATION
WHERE CITY REGEXP '^[aeiou].*[aeiou]$';

<br />
<h6>Weather Observation Station 9</h6>
SELECT DISTINCT CITY FROM STATION
WHERE NOT CITY REGEXP '^[aeiou]';

<br />
<h6>Weather Observation Station 10</h6>
SELECT DISTINCT CITY FROM STATION
WHERE NOT CITY REGEXP '[aeiou]$'


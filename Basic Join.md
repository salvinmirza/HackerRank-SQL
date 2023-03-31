<h6> Learning Resource </h6>
https://www.youtube.com/watch?v=9yeOJ0ZMUYw&ab_channel=Socratica
<br />

<h6>Population Census</h6>

```sql

  SELECT SUM(City.population)
  FROM City
  INNER JOIN Country ON City.CountryCode = Country.Code
  WHERE Country.Continent = 'Asia'

```
<br />

<h6>African Cities</h6>

```sql

  SELECT CITY.NAME
  FROM CITY
  INNER JOIN Country ON City.CountryCode = Country.Code
  WHERE Country.Continent = 'Africa'

```
<br />

<h6>Average Population of Each Continent</h6>

```sql

  SELECT Country.Continent, FLOOR(AVG(City.Population))
  FROM City 
  INNER JOIN Country ON City.CountryCode = Country.Code
  GROUP BY Country.Continent ;

```

<br />

<h6>The Report</h6>

```sql

  SELECT IF(GRADES.GRADE>=8, STUDENTS.NAME, NULL),GRADES.GRADE, STUDENTS.MARKS
  FROM GRADES, STUDENTS
  WHERE STUDENTS.MARKS BETWEEN GRADES.MIN_MARK AND GRADES.MAX_MARK
  ORDER BY GRADES.GRADE DESC, STUDENTS.NAME;

```
<br />

<h6>Top Competitors</h6>

```sql

    SELECT
      h.hacker_id, h.name
  FROM
      hackers h
      JOIN submissions s ON h.hacker_id = s.hacker_id
      JOIN challenges c ON s.challenge_id = c.challenge_id
      JOIN difficulty d ON c.difficulty_level = d.difficulty_level AND s.score = d.score
  GROUP BY
      h.hacker_id,
      h.name
  HAVING
      COUNT(c.challenge_id) > 1
  ORDER BY
      COUNT(c.challenge_id) DESC,
      h.hacker_id

```

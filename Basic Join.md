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

  SELECT CITY.NAME
  FROM CITY
  INNER JOIN Country ON City.CountryCode = Country.Code
  WHERE Country.Continent = 'Africa'

```

<h6>Population Census</h6>

```sql

  SELECT SUM(City.population)
  FROM City
  INNER JOIN Country ON City.CountryCode = Country.Code
  WHERE Country.Continent = 'Asia'

```

```shell
SHOW DATABASES;

USE WORLD;

SHOW TABLES;

DESC city;

SELECT COUNT(city.Name) AS 'Cities in The USA'
FROM city
WHERE city.CountryCode = 'USA'
;


SELECT country.Name AS Country, country.Population, country.LifeExpectancy
FROM country
WHERE country.Code = 'ARG'
;

SELECT city.Name AS 'Cities in Russia'
FROM city
WHERE city.CountryCode = 'RUS'
;

SELECT *
FROM city
WHERE city.Name LIKE 'A__M%'
;

SELECT COUNT(countrylanguage.Language) AS 'Number of Countries Where Spoken', countrylanguage.Language
FROM countrylanguage
GROUP BY countrylanguage.Language
ORDER BY countrylanguage.Language
;

```
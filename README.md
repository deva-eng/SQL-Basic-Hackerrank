# SQL-Basic-Hackerrank
Here the questions and solution (LANGUAGE - ORACLE) for the sql basics will be provided...There are can be other solutions but these are the ones I approached with....

QUESTION 1 - Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA.

SOLUTION - select * from CITY where population>100000 and countrycode='USA'; 

QUESTION 2 - Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA.

SOLUTION - select name from city where population>120000 and countrycode='USA';

QUESTION 3 - Query all columns (attributes) for every row in the CITY table.

SOLUTION - select * from city;

QUESTION 4 - Query all columns for a city in CITY with the ID 1661.

SOLUTION - select * from city where id=1661;

QUESTION 5 - Query all attributes of every Japanese city in the CITY table. The COUNTRYCODE for Japan is JPN.

SOLUTION - select * from city where countrycode='JPN';

QUESTION 6 - Query the names of all the Japanese cities in the CITY table. The COUNTRYCODE for Japan is JPN.

SOLUTION - select name from city where countrycode='JPN';

QUESTION 7 - Query a list of CITY and STATE from the STATION table.

SOLUTION - select city, state from station;

QUESTION 8 - Query a list of CITY names from STATION for cities that have an even ID number. Print the results in any order, but exclude duplicates from the answer.

SOLUTION - select distinct city from station where mod(id,2)=0;

QUESTION 9 - Find the difference between the total number of CITY entries in the table and the number of distinct CITY entries in the table.

SOLUTION - select count(city)-count(distinct city) from station;

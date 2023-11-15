# week-10
week-10 sql exercises

## Assesment 1
### Question 1
SELECT title, description FROM film;

### Question 2
SELECT * FROM film
WHERE length > 60 AND length < 75;

### Question 3
SELECT * FROM film
WHERE rental_rate = 0.99 AND (replacement_cost = 12.99 OR replacement_cost = 28.99);

### Question 4
SELECT last_name FROM customer
WHERE first_name = 'Mary';

### Question 5
SELECT * FROM film
WHERE NOT length > 50 AND NOT (rental_rate = 2.99 OR rental_rate = 4.99);

## Assesment 2
### Question 1
SELECT * FROM film
WHERE replacement_cost BETWEEN 12.99 AND 16.99;

### Question 2
SELECT first_name, last_name FROM actor
WHERE first_name IN ('Penelope', 'Nick', 'Ed');

### Question 3
SELECT * FROM film
WHERE rental_rate IN (0.99, 2.99, 3.99) AND replacement_cost IN (12.99, 15.99, 28.99);

## Assesment 3
### Question 1
SELECT country FROM country 
WHERE country LIKE 'A%a';

### Question 2
SELECT country FROM country 
WHERE country LIKE '%_____n';

### Question 3
SELECT title FROM film 
WHERE title ILIKE 't%t%t%t%' OR title ILIKE '%t%t%t%t%';

### Question 4
SELECT * FROM film
WHERE title LIKE 'C%' AND length > 90 AND rental_rate = 2.99;

## Assesment 4
### Question 1
SELECT DISTINCT replacement_cost FROM film;

### Question 2
SELECT COUNT (DISTINCT replacement_cost) FROM film;

### Question 3
SELECT COUNT (*) FROM film
WHERE title LIKE 'T%' AND rating = 'G';

### Question 4
SELECT COUNT (*) FROM country
WHERE country LIKE '_____';

### Question 5
SELECT COUNT (*) FROM city
WHERE city ILIKE '%r';

# Subtask 1
Szczerze mówiąc nie ogładałam tego szkolenia, ponieważ wcześniej już przechodziłam miniszkolenie z SQL :D jestem trochę "rusty", ale ogólnie w miarę dobrze się czuję w stosowaniu operatorów typu: AND, IN, BETWEEN, LIKE, OR, WHERE itd. 
Jak zawsze powtarzał nasz szkoleniowiec: SELECT (gwiazdka) FROM tabela będziesz mistrzem sqla ;)

# Subtask 3
1.  Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname 
2. -- → SELECT * FROM actors ORDER BY surname;--
3.  Wyświetl film, który powstał w 2019 roku 
4.  → SELECT * FROM movies WHERE (year_of_production) = 2019; 
5.  Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem 
6.  → SELECT * FROM movies WHERE (year_of_production) BETWEEN 1900 AND 1999;
7.  Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$; 
8.  → SELECT title, price FROM movies WHERE price < 7;
9.  Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN 
10.  → SELECT * FROM actors WHERE actor_id >= 4 AND actor_id <= 7;
11.  Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny 
12.  → SELECT * FROM customers WHERE customer_id = 2 OR customer_id = 4 OR customer_id = 6;
13.  Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN 
14.  → SELECT * FROM customers WHERE customer_id IN (1, 3, 5);
15.  Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An” 
16.  → SELECT * FROM actors WHERE first_name LIKE 'An%';
17.  Wyświetl dane klienta, który nie ma podanego adresu email 
18.  → SELECT customer_id, name, surname FROM customers WHERE email IS NULL;
19. Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id 
20. → SELECT movie_id, title, price FROM movies WHERE price > 9 AND movie_id BETWEEN 2 AND 8;




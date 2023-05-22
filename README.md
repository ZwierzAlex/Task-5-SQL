# Subtask 1
Szczerze mówiąc nie ogładałam tego szkolenia, ponieważ wcześniej już przechodziłam miniszkolenie z SQL :grinning: jestem trochę "rusty", ale ogólnie w miarę dobrze się czuję w stosowaniu operatorów typu: AND, IN, BETWEEN, LIKE, OR, WHERE itd. <br>
Jak zawsze powtarzał nasz szkoleniowiec: ***SELECT (gwiazdka) FROM tabela będziesz mistrzem sqla :rofl:***

# Subtask 3
1.  *Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname* 
    __→ SELECT * FROM actors ORDER BY surname;__
2.  *Wyświetl film, który powstał w 2019 roku*
    __→ SELECT * FROM movies WHERE (year_of_production) = 2019;__ 
3.  *Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem*
    __→ SELECT * FROM movies WHERE (year_of_production) BETWEEN 1900 AND 1999;__
4.  *Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$;* 
    __→ SELECT title, price FROM movies WHERE price < 7;__
5.  *Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN* 
     __→ SELECT * FROM actors WHERE actor_id >= 4 AND actor_id <= 7;__
6.  *Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny* 
    __→ SELECT * FROM customers WHERE customer_id = 2 OR customer_id = 4 OR customer_id = 6;__
7.  *Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN* 
    __→ SELECT * FROM customers WHERE customer_id IN (1, 3, 5);__
8.  *Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”* 
    __→ SELECT * FROM actors WHERE first_name LIKE 'An%';__
9.  *Wyświetl dane klienta, który nie ma podanego adresu email* 
    __→ SELECT customer_id, name, surname FROM customers WHERE email IS NULL;__
10. *Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id* 
    __→ SELECT movie_id, title, price FROM movies WHERE price > 9 AND movie_id BETWEEN 2 AND 8;__




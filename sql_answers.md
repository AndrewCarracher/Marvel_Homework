Questions

Return ALL the data in the 'movies' table.

SELECT * FROM movies;

1	Iron Man	2008	15:35
2	The Incredible Hulk	2008	22:05
3	Iron Man 2	2010	18:00
4	Thor	2011	21:20
5	Captain America: The First Avenger	2011	13:10
6	Avengers Assemble	2012	14:30
7	Iron Man 3	2013	21:55
8	Thor: The Dark World	2013	15:20
9	Batman Begins	2005	20:30
10	Captain America: The Winter Soldier	2014	21:10
11	Guardians of the Galaxy	2014	16:20
12	Avengers: Age of Ultron	2015	23:00
13	Ant-Man	2015	13:25
14	Captain America: Civil War	2016	14:45
15	Doctor Strange	2016	22:40
16	Guardians of the Galaxy 2	2017	22:00
17	Spider-Man: Homecoming	2017	18:10
18	Thor: Ragnarok	2017	19:35
19	Black Panther	2018	22:20

Return ONLY the name column from the 'people' table

SELECT name FROM people

Ana Martinez
Andrew Carracher
Caroline Graves
Genna-Lee Walsh
Graham Stein
Iain Floyd
Iona Wright
Jackie Farr
Jennifer Proctor
Jordan Raitt
Katherine Jeffree
Kris McElhinney
Michael Griffin
Monica Mateiu
Nathan Atkinson
Nyalls Hemingway
Oksana Richards
Rana Akbar
Tavy Fraser
Thomas Gracie
Xavier Godard
Kith Douglas

Oops! Someone at CodeClan spelled Keith's name wrong! Change it to reflect the proper spelling.

UPDATE people
SET name = 'Keith'
WHERE id = 22;

UPDATE 1

Return ONLY your name from the 'people' table.

SELECT name FROM people
WHERE name = 'Andrew Carracher';

Andrew Carracher

The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.


DELETE FROM movies
WHERE id = 9

DELETE 1

Create a new entry in the 'people' table with the name of one of the instructors.

INSERT INTO people (name) VALUES ('Craig Morton');

INSERT 0 1

Pawel has decided to hijack our movie evening, Remove him from the table of people.

DELETE FROM people
where id = 24

DELETE 1

The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this.

INSERT INTO movies (title, year, show_time) VALUES ('Avengers: Infinity War, 2018, '00:00');

INSERT 0 1

The cinema would also like to make the Guardians movies a back to back feature. Find out the show time of "Guardians of the Galaxy" and set the show time of "Guardians of the Galaxy 2" to start two hours later.
Extension

SELECT show_time FROM movies WHERE title = 'Guardians of the Galaxy'

16:20

UPDATE movies SET show_time = '18:20' WHERE title = 'Guardians of the Galaxy 2'

UPDATE 1

Delete multiple entries from your table in a single command.

DELETE FROM people
WHERE name LIKE '%ac%'

DELETE 3

Select all the movies ordered by year in descending order

SELECT * FROM movies
ORDER BY year DESC

20	Avengers: Infinity War	2018	24:00
19	Black Panther	2018	22:20
16	Guardians of the Galaxy 2	2017	18:20
18	Thor: Ragnarok	2017	19:35
17	Spider-Man: Homecoming	2017	18:10
15	Doctor Strange	2016	22:40
14	Captain America: Civil War	2016	14:45
13	Ant-Man	2015	13:25
12	Avengers: Age of Ultron	2015	23:00
11	Guardians of the Galaxy	2014	16:20
10	Captain America: The Winter Soldier	2014	21:10
8	Thor: The Dark World	2013	15:20
7	Iron Man 3	2013	21:55
6	Avengers Assemble	2012	14:30
5	Captain America: The First Avenger	2011	13:10
4	Thor	2011	21:20
3	Iron Man 2	2010	18:00
2	The Incredible Hulk	2008	22:05
1	Iron Man	2008	15:35

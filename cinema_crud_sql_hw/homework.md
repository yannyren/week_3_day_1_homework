

## Questions

1. Return ALL the data in the 'movies' table.
SELECT * FROM movies;

2. Return ONLY the name column from the 'people' table
SELECT name FROM people

3. Oops! Someone at CodeClan spelled Del's name wrong! Change it to reflect the proper spelling.
UPDATE people SET name = 'Derek Middlemiss' WHERE name = 'Del Boy Middlemiss';

4. Return ONLY your name from the 'people' table.
SELECT name FROM people WHERE name = 'Yan Ren';

5. The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.
DELETE FROM movies WHERE title = 'Batman Begins';

6. Create a new entry in the 'people' table with the name of one of the instructors.
INSERT INTO people (name) VALUES ('Keith');

7. John Travolta, has decided to hijack our movie evening, Remove him from the table of people.
DELETE FROM people WHERE name = 'John Travolta';

8. Somehow the list of people includes two people named 'Christopher'. Change these entries to the proper names ('Christopher Whatshisface', 'Christopher Theotherone')
UPDATE people SET name = 'Christopher Whatshisface' WHERE name = 'Christopher Donnelly';
UPDATE people SET name = 'Christopher Theotherone' WHERE name = 'Christopher Hunter';

9. The cinema has just heard that they will be holding an exclusive midnight showing of 'Guardians of the Galaxy 2'!! Create a new entry in the 'movies' table to reflect this.
INSERT INTO movies (title, year, show_time) VALUES ('Guardians of the Galaxy 2', 2017, '24:00');

10. The cinema would also like to make the Guardian movies a back to back feature. Update the 'Guardians of the Galaxy' show time from 12:10 to 21:30
UPDATE movies SET show_time = '21:30' WHERE title = 'Guardians of the Galaxy';

## Extension

1. Research how to delete multiple entries from your table in a single command.
DELETE FROM people WHERE id BETWEEN 1 AND 4
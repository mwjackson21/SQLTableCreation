# SQLTableCreation
This SQL code demonstrates various database operations using an example table named 'friends.' These operations include creating a table, inserting data, updating records, altering the table structure, and deleting records. Below, we explain each part of the code and how to use it.

Table Creation
The code begins by creating a table called 'friends' with three columns: 'id' (an INTEGER), 'name' (TEXT), and 'birthday' (DATE).

CREATE TABLE friends (
  id INTEGER,
  name TEXT,
  birthday DATE
);
- This SQL statement defines the structure of the 'friends' table.

Data Insertion
Next, data is inserted into the 'friends' table using INSERT statements:

INSERT INTO friends (id, name, birthday)
VALUES (1, 'Ororo Munroe', '1940-05-30');

INSERT INTO friends (id, name, birthday)
VALUES (2, 'Norman Reedus', '1969-01-06');

INSERT INTO friends (id, name, birthday)
VALUES (3, 'Pedro Pascal', '1975-04-02');
- These statements insert three rows of data into the 'friends' table, providing values for 'id,' 'name,' and 'birthday' columns.

Data Updates
The code then demonstrates how to update existing records:

UPDATE friends
SET name = 'Storm'
WHERE id = 1;
- This statement updates the 'name' column for the record with 'id' 1 to 'Storm.'

Alter Table
The 'ALTER TABLE' statement adds a new column 'email' of type TEXT to the 'friends' table:

ALTER TABLE friends
ADD COLUMN email TEXT;
- This statement modifies the table structure by adding a new column 'email' to store email addresses.

More Data Updates
Following the alteration of the table, the code updates email addresses for specific records:

UPDATE friends
SET email = 'storm@codecademy.com'
WHERE id = 1;

UPDATE friends
SET email = 'NormanReedus@gmail.com'
WHERE id = 2;

UPDATE friends
SET email = 'PedroPascal@gmail.com'
WHERE id = 3;
- These statements assign email addresses to 'email' column for 'id' 1, 2, and 3 respectively.

Data Deletion
Finally, the code demonstrates how to delete a record from the 'friends' table:

DELETE FROM friends
WHERE id = 1;
- This statement deletes the record with 'id' 1 from the 'friends' table.

Viewing Data
To view the data in the 'friends' table at any point, you can use the SELECT statement:

SELECT *
FROM friends;
- This statement retrieves all rows and columns from the 'friends' table.

# SQL-Query-Log
Here's a log of my SQL skillset!

# Distinct
Used to return a liust of unique values per row.

Example query:<br/>
SELECT distinct author, genre<br/>
FROM book;<br/>

# Aliasing
Use alias to rename columns.

Example query:<br/>
SELECT name AS first_name, year_hired<br/>
FROM Employees<br/>

# Views

A view is a virtual table that is the result of a saved SQL SELECT statement.
Data in a view is not generally stored in a database. When it's accessed, views generally update in response to update in response to updates in the underlying data.

Example query:<br/>
CREATE VIEW employee_hire_years AS<br/>
SELECT id, name, year_hired<br/>
FROM employees;<br/>

Once it's created, it can be queried like how we query a normal table.

SELECT id, name, year_hired FROM employee_hire_years<br/>

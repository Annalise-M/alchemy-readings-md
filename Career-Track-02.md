Reading Notes - Career Track 02
---

Inside a Computer
@ https://edu.gcfglobal.org/en/computerbasics/inside-a-computer/1/

The hardware of a computer consists of the following: 

    Motherboard - main curcuit board (brain of computer)

    CPU/Processor - central processing unit

    RAM - random access memory 
    the short term memory of the computer

    Hard drive - long term storage of the computer

    Power Supply Unit - converts wall plug in for power by the computer

    Expansion Cards - boosts computer performance ie. video cards, sound cards, bluetooth card etc. 

    (see link above for more info.)

PostgresSQL INSERT -
    @ https://www.postgresqltutorial.com/postgresql-insert/

    allows you to insert a new row into a table

    INSERT INTO table_name(column1, column2, …)
    VALUES (value1, value2, …);

PostgresSQL SELECT -
    @ https://www.postgresqltutorial.com/postgresql-select/

    The SELECT statement has the following clauses:

    Select distinct rows using DISTINCT operator.
    Sort rows usingORDER BY clause.
    Filter rows using WHERE clause.
    Select a subset of rows from a table using LIMIT or FETCH clause.
    Group rows into groups using GROUP BY clause.
    Filter groups using HAVING clause.
    Join with other tables using joins such as INNER JOIN, LEFT JOIN, FULL OUTER JOIN, CROSS JOIN clauses.
    Perform set operations using UNION, INTERSECT, and EXCEPT.

    SELECT
        select_list
    FROM
        table_name;

PostgresSQL UPDATE -
    @ https://www.postgresqltutorial.com/postgresql-update/

    UPDATE statement allows you to modify data in a table

    UPDATE table_name
    SET column1 = value1,
        column2 = value2,
        ...
    WHERE condition;


PostgresSQL DELETE -
    @ https://www.postgresqltutorial.com/postgresql-delete/

    DELETE statement allows you to delete one or more rows from a table.
    ---
    DELETE FROM table_name
    WHERE condition;
    ---
    First, specify the name of the table from which you want to delete data after the DELETE FROM keywords.

    Second, use a condition in the WHERE clause to specify which rows from the table to delete.

    The WHERE clause is optional. If you omit the WHERE clause, the DELETE statement will delete all rows in the table.

    The DELETE statement returns the number of rows deleted. It returns zero if the DELETE statement did not delete any row.

    To return the deleted row(s) to the client, you use the RETURNING clause as follows:

    ---
    DELETE FROM table_name
    WHERE condition
    RETURNING (select_list | *)
    ---
    
# SQL Concepts Explained (Beginner → Pro)

A clean, simple SQL table covering **DQL, DML, DDL, DCL**, operators,
joins, functions, and window functions with sample queries.

------------------------------------------------------------------------

## 📌 SQL Command Categories Table

  ------------------------------------------------------------------------------------------------------------------------
  Category       Command        Meaning        Example Query
  -------------- -------------- -------------- ---------------------------------------------------------------------------
  **DQL**        SELECT         Fetch data     `SELECT * FROM employees;`
                                from table     

  **DQL**        WHERE          Filter rows    `SELECT * FROM employees WHERE salary > 50000;`

  **DQL**        GROUP BY       Group rows     `SELECT dept, COUNT(*) FROM employees GROUP BY dept;`

  **DQL**        HAVING         Filter after   `SELECT dept, COUNT(*) FROM employees GROUP BY dept HAVING COUNT(*) > 5;`
                                grouping       

  **DQL**        ORDER BY       Sort data      `SELECT * FROM employees ORDER BY salary DESC;`
  ------------------------------------------------------------------------------------------------------------------------

------------------------------------------------------------------------

## 📌 SQL DML (Data Manipulation Language)

  ------------------------------------------------------------------------------------------------------------------
  Command            Meaning            Example Query
  ------------------ ------------------ ----------------------------------------------------------------------------
  **INSERT**         Add data           `INSERT INTO employees (name, dept, salary) VALUES ('John', 'IT', 60000);`

  **UPDATE**         Modify data        `UPDATE employees SET salary = 65000 WHERE name='John';`

  **DELETE**         Remove data        `DELETE FROM employees WHERE name='John';`

  **SELECT**         Read data          `SELECT * FROM employees;`
  ------------------------------------------------------------------------------------------------------------------

------------------------------------------------------------------------

## 📌 SQL DDL (Data Definition Language)

  --------------------------------------------------------------------------------------------
  Command            Meaning            Example Query
  ------------------ ------------------ ------------------------------------------------------
  **CREATE**         Create             `CREATE TABLE employees (id INT, name VARCHAR(50));`
                     database/table     

  **ALTER**          Modify table       `ALTER TABLE employees ADD COLUMN dept VARCHAR(20);`

  **DROP**           Delete table or    `DROP TABLE employees;`
                     database           

  **TRUNCATE**       Remove all rows    `TRUNCATE TABLE employees;`
  --------------------------------------------------------------------------------------------

------------------------------------------------------------------------

## 📌 SQL DCL (Data Control Language)

  --------------------------------------------------------------------------------
  Command            Meaning            Example Query
  ------------------ ------------------ ------------------------------------------
  **GRANT**          Give permission    `GRANT SELECT ON employees TO user1;`

  **REVOKE**         Remove permission  `REVOKE SELECT ON employees FROM user1;`
  --------------------------------------------------------------------------------

------------------------------------------------------------------------

## 📌 SQL Operators

  Operator      Meaning               Example
  ------------- --------------------- ----------------------------------
  **=**         Equal                 `salary = 50000`
  **\>**        Greater than          `salary > 50000`
  **\<**        Lesser than           `salary < 40000`
  **BETWEEN**   Range                 `salary BETWEEN 40000 AND 60000`
  **IN**        Match value in list   `dept IN ('IT', 'HR')`
  **LIKE**      Pattern match         `name LIKE 'A%'`
  **AND, OR**   Combine conditions    `dept='IT' AND salary>50000`

------------------------------------------------------------------------

## 📌 SQL JOINS

  ----------------------------------------------------------------------------------------------------------------------------
  Join Type                   Meaning                Example
  --------------------------- ---------------------- -------------------------------------------------------------------------
  **INNER JOIN**              Match rows in both     `SELECT e.name, d.dept FROM emp e INNER JOIN dept d ON e.dept_id=d.id;`
                              tables                 

  **LEFT JOIN**               Keep left table +      `SELECT * FROM emp LEFT JOIN dept ON ...`
                              matching right         

  **RIGHT JOIN**              Keep right table +     `SELECT * FROM emp RIGHT JOIN dept ON ...`
                              matching left          

  **FULL JOIN**               All rows from both     `SELECT * FROM emp FULL JOIN dept ON ...`
                              sides                  
  ----------------------------------------------------------------------------------------------------------------------------

------------------------------------------------------------------------

## 📌 SQL Functions

  Function      Use              Example
  ------------- ---------------- --------------------------------------
  **COUNT()**   Number of rows   `SELECT COUNT(*) FROM employees;`
  **SUM()**     Total            `SELECT SUM(salary) FROM employees;`
  **AVG()**     Average          `SELECT AVG(salary) FROM employees;`
  **MAX()**     Highest value    `SELECT MAX(salary) FROM employees;`
  **MIN()**     Lowest value     `SELECT MIN(salary) FROM employees;`

------------------------------------------------------------------------

## 📌 Window Functions

  ---------------------------------------------------------------------------------------------
  Function                  Meaning                Example
  ------------------------- ---------------------- --------------------------------------------
  **ROW_NUMBER()**          Ranking                `ROW_NUMBER() OVER (ORDER BY salary DESC)`

  **RANK()**                Ranking with gaps      `RANK() OVER (ORDER BY salary DESC)`

  **DENSE_RANK()**          Ranking without gaps   `DENSE_RANK() OVER (ORDER BY salary DESC)`

  **LAG()**                 Previous row value     `LAG(salary,1) OVER (ORDER BY id)`

  **LEAD()**                Next row value         `LEAD(salary,1) OVER (ORDER BY id)`

  **NTILE()**               Bucketing              `NTILE(4) OVER (ORDER BY salary)`
  ---------------------------------------------------------------------------------------------

------------------------------------------------------------------------

## 📌 Aliases

  ---------------------------------------------------------------------------------------------------
  Feature                 Meaning                 Example
  ----------------------- ----------------------- ---------------------------------------------------
  **AS**                  Rename column/table     `SELECT salary AS monthly_salary FROM employees;`

  ---------------------------------------------------------------------------------------------------

------------------------------------------------------------------------

## 📌 Wildcards

  Symbol       Meaning                    Example
  ------------ -------------------------- --------------------------------------
  **%**        Any number of characters   `'A%'` → starts with A
  \*\*\_\*\*   Single character           `'A_'` → starts with A & 1 more char

------------------------------------------------------------------------

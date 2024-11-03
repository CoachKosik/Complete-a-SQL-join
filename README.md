# Complete a SQL join

## Objective

This lab aims to introduce the concept of SQL joins and provide hands-on experience in combining data from multiple tables. By mastering SQL joins, users can effectively extract and analyze complex datasets, enabling them to conduct in-depth security investigations and make informed decisions.

## Project description

This project focuses on utilizing SQL joins to combine data from multiple tables. By mastering inner, left, and right joins, users can effectively analyze complex datasets and gain valuable insights. This skill is crucial for security analysts who need to correlate information from different sources to investigate security incidents and identify potential threats.

## Skills Learned

* **SQL Joins:** Understanding and applying different types of joins (inner, left, right) to combine data from multiple tables.
* **Data Relationships:** Identifying relationships between tables and selecting appropriate join types to extract relevant information.
* **Complex Queries:** Constructing complex SQL queries involving multiple tables and conditions.
* **Data Analysis:** Interpreting joined data to identify patterns, anomalies, and potential security threats.

By mastering these skills, users can effectively analyze large and complex datasets, enabling you to make informed decisions and respond to security incidents efficiently.

## Tools Used

* **SQL Database:** A database management system used to store and manage structured data.
* **SQL Query Language:** Used to interact with the database and retrieve specific information.
* **MariaDB Shell:** A command-line interface for interacting with the MariaDB database.

By utilizing these tools and SQL's join operations (INNER JOIN, LEFT JOIN, RIGHT JOIN), users can effectively combine data from multiple tables, enabling comprehensive analysis and informed decision-making.

## Steps
1. Match employees to their machines
* First, you must identify which employees are using which machines. The data is located in the machines and employees tables.
  * You must use a SQL inner join to return the records you need based on a connecting column. In the scenario, both tables include the device_id column, which you’ll use to perform the join.
    * Run a query to retrieve all records from the machines table:
    * ![join 1](https://github.com/user-attachments/assets/df9e4193-dbea-4c7f-b689-f53a451389fa)
  * You’ll note that this query is not sufficient to perform the join and retrieve the information you need.
    * Complete the query to perform an inner join between the machines and employees tables on the device_id column.
      *  To complete a join you need to link the joined tables on a common column. In the case of the employees and machines tables, the device_id column is common.
      *  ![join 3](https://github.com/user-attachments/assets/a4ad1b59-78d7-4a43-b6bd-eccb2a2189fe)
      
2. Return more data
* You now must return the information on all machines and the employees who have machines. Next, you must do the reverse and retrieve the information of all employees and any machines that are assigned to them.
* To achieve this, you’ll complete a left join and a right join on the employees and machines tables. The results will include all records from one or the other table. You must link these tables using the common device_id column.
  * Run a SQL query to connect the machines and employees tables through a left join.
    * ![image](https://github.com/user-attachments/assets/35597bfd-34a8-4e2d-9570-81af5ec6ace2)
  * Run a SQL query to connect the machines and employees tables through a right join.
    * ![join 6](https://github.com/user-attachments/assets/caa3eacd-369e-4ccb-9b52-3f8404c104ef)

3. Retrieve login attempt data
* To continue investigating the security incident, you must retrieve the information on all employees who have made login attempts. To achieve this, you’ll perform an inner join on the employees and log_in_attempts tables, linking them on the common username column.
  * Run a SQL query to perform an inner join on the employees and log_in_attempts tables.
    * ![join 7](https://github.com/user-attachments/assets/94ca22cd-fe5a-496e-95bd-96c83807f2bf)

### Summary

This activity provided hands-on experience in utilizing SQL joins to combine data from multiple tables. By effectively employing INNER JOIN, LEFT JOIN, and RIGHT JOIN, users can extract comprehensive and relevant information, enabling in-depth analysis and informed decision-making.

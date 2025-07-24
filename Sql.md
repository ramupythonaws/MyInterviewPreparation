Here are **100 SQL questions** covering basic, intermediate, and advanced concepts, including theoretical questions and hands-on query exercises. Only questions are listed (no answers), as requested.

### Basic Level (1-35)

1. What is SQL?
2. What are the different types of SQL statements?
3. Explain the difference between SQL and MySQL.
4. What is a table in SQL?
5. Define a field (column) in SQL.
6. What is a primary key?
7. What is a foreign key?
8. What is a unique key?
9. What is a constraint? Name different types of constraints.
10. What are DDL, DML, DCL, and TCL commands?
11. How do you retrieve all records from a table?
12. Write a query to select only specific columns from a table.
13. How do you filter data in SQL using the WHERE clause?
14. How do you use the ORDER BY clause in SQL?
15. How do you use the GROUP BY clause in SQL?
16. How do you use the HAVING clause in SQL?
17. What is the BETWEEN operator in SQL?
18. How do you use the LIKE operator? Give one example.
19. What does the IN operator do?
20. Explain the purpose of the DISTINCT keyword.
21. What is a NULL value? How is it different from zero or blank?
22. What is an alias in SQL? How do you define one?
23. What is the function of aggregate functions? Name at least three.
24. Differentiate between COUNT(*) and COUNT(column).
25. What is a JOIN? List the different types of JOINs in SQL.
26. Write a query for INNER JOIN between two tables.
27. What is a LEFT JOIN? Provide an example use case.
28. What is a RIGHT JOIN? Provide an example use case.
29. What is a FULL OUTER JOIN?
30. What is a CROSS JOIN?
31. Write a query to update records in a table.
32. Write a query to delete records from a table.
33. Write a query to add a new column to an existing table.
34. Explain how to remove a column from a table.
35. How do you rename a table in SQL?

### Intermediate Level (36-70)

36. Explain normalization and why it is important.
37. Describe the first, second, and third normal forms (1NF, 2NF, 3NF).
38. What is denormalization?
39. What is an index? Why and when should you create indexes?
40. What is a view? How is it different from a table?
41. How do you create a view in SQL?
42. How do you update data through a view?
43. What are subqueries? Provide an example.
44. What is a correlated subquery?
45. Explain the use of EXISTS and NOT EXISTS.
46. What is the difference between WHERE and HAVING?
47. What is the difference between UNION and UNION ALL?
48. Write a query to find duplicate records in a table.
49. Write a query to remove duplicate records from a table.
50. What is a stored procedure?
51. How do you call a stored procedure?
52. What is a function in SQL, and how is it different from a stored procedure?
53. What is a trigger? When would you use one?
54. Describe the differences between clustered and non-clustered indexes.
55. What are transactions in SQL? Explain ACID properties.
56. What is a savepoint in a transaction?
57. Write a query to find the second highest salary from an employee table.
58. Write a query to list employees whose names start with ‘A’.
59. Write a query to calculate total sales per region.
60. How do you find the number of orders placed on each day?
61. How do you update all salaries by 10% for employees with a salary below 50000?
62. Write a query to select all customers who have placed no orders.
63. How do you delete records in one table based on conditions in another table?
64. What is a self join? Give a practical example.
65. Write a query using CASE for conditional output.
66. What is the COALESCE function? When would you use it?
67. Write a query to pivot data (convert rows to columns).
68. Explain the use of window functions.
69. Write a query using RANK() or DENSE_RANK().
70. What is the default sorting order of ORDER BY in SQL?

### Advanced Level (71-100)

71. Explain the concept of window frames in window functions.
72. Write a query using LEAD() or LAG() to compare current and previous row values.
73. What is CTE (Common Table Expression)? Give an example.
74. Explain recursive queries using CTE.
75. How do you handle errors in SQL procedures?
76. What is dynamic SQL?
77. What are materialized views? How do they differ from regular views?
78. Explain database partitioning and its benefits.
79. How do you perform bulk data inserts efficiently?
80. What is a deadlock? How do you investigate and resolve deadlocks?
81. Write a query to find continuous dates in a date column without gaps.
82. Write a query to get top N records per group (e.g., top 3 orders per customer).
83. What is horizontal vs vertical partitioning?
84. How do you implement soft delete in a table?
85. Write a query to calculate a running total.
86. What is the isolation level in transactions? Name all standard levels.
87. How do you optimize a slow SQL query?
88. How do you identify missing indexes in a database?
89. Explain the difference between DELETE, TRUNCATE, and DROP.
90. Write a query to transpose a table (swap rows and columns).
91. What is the role of system tables/information_schema in SQL?
92. How do you generate test data in SQL?
93. How do you export table data to a file using SQL?
94. What is database sharding?
95. How would you encrypt a column in SQL Server or PostgreSQL?
96. What are temporal tables? When would you use them?
97. Write a query to unpivot data (columns to rows).
98. Explain optimistic vs pessimistic locking.
99. What are surrogate keys? Why might you use them over natural keys?
100. Write a SQL query or approach to resolve the N+1 query problem in reporting.

# Related
What are the fundamental SQL commands everyone should know
How do you perform different types of joins in SQL with examples
Can you write a query to find duplicate records in a table
What is the purpose of constraints like PRIMARY KEY and FOREIGN KEY in SQL
How can you optimize a slow-running SQL query



Here is a curated list of **100 SQL exercise questions** focused specifically on **JOINS, GROUP BY, and HAVING** clauses, designed to cover from basic to advanced levels. These exercises emphasize practical query writing and data analysis skills.

### SQL JOINS Exercises (1-50)

1. Write a query to list all salespersons and customers who live in the same city.  
2. Retrieve all orders with customer names using INNER JOIN between Orders and Customers.  
3. Write a query to find all employees with their department names using an INNER JOIN.  
4. Display all employees along with their managers’ names using a self JOIN.  
5. List all customers and their orders including those customers who have no orders (LEFT JOIN).  
6. List all departments and any employees in them, including departments with no employees (RIGHT JOIN).  
7. Write a query to find customers who have not made any orders using LEFT JOIN.  
8. Display all products along with their suppliers, including products without suppliers (FULL OUTER JOIN).  
9. Find the total number of orders made by each customer using JOIN and GROUP BY.  
10. Write a query to show employees and their project names, including employees not assigned to any project (LEFT JOIN).  
11. Write a query to find employees whose salaries are less than their managers’ salaries using a self JOIN.  
12. Retrieve the list of customers along with the last order date using JOIN and GROUP BY.  
13. Write a query to find products that have never been ordered using LEFT JOIN.  
14. Combine two tables containing artist and album information using JOIN on the artist_id key.  
15. Write a query to list the top 3 customers with the highest total order amounts using JOIN, GROUP BY, and ORDER BY.  
16. Find all employees who work in the ‘Sales’ department using JOIN and WHERE clause.  
17. Write a JOIN query to display student names and the courses they are enrolled in.  
18. Write a query to show all suppliers and the categories they supply, even if the category has no supplier (FULL JOIN).  
19. Use JOIN to list all employees and their job titles.  
20. Write a query to find departments where no employees report to the manager.  
21. Return the first name and last name of employees and their managers using a self JOIN with aliases.  
22. Write a JOIN query that lists customers and the products they purchased, with product details.  
23. Find all orders placed along with the shipping company details using JOIN.  
24. Write a query to display customers who placed an order in 2024 using JOIN and WHERE clause on OrderDate.  
25. Write a query to select all employees who earn more than their department’s average salary using JOIN and GROUP BY.  
26. List all distinct cities where at least one salesman and customer live using JOIN.  
27. Write a query to match customers with salespersons based on matching city values using JOIN.  
28. Retrieve employees along with the name of the department and location using multiple JOINs.  
29. Write a query to find the number of products supplied by each supplier using JOIN and GROUP BY.  
30. Display customer names along with the total number of orders they have placed using JOIN and aggregation.  
31. Write a query to display student and teacher names where the students and teachers belong to the same subject.  
32. Retrieve list of employees and their corresponding commission rates using JOIN.  
33. Write a query to list employees who do not have a manager using LEFT JOIN.  
34. Find all customers who placed orders that have not been shipped yet using JOIN.  
35. Display all products along with the total quantity sold using JOIN, GROUP BY, and SUM.  
36. Write a query to list all employees with their department names and location names.  
37. Find all customers and their last order date using JOIN and GROUP BY.  
38. Write a query to show product names and the total sale amount for each product using JOIN and aggregation.  
39. List all orders and the customers who placed them, including orders without customer information (RIGHT JOIN).  
40. Write a query to find employees who switched projects between two time periods using JOIN and date range conditions.  
41. Find all pairs of employees who work on the same project using self JOIN.  
42. Write a query to list all products with more than 10 orders using JOIN and HAVING.  
43. Retrieve all customers along with the average order quantity using JOIN, GROUP BY, and AVG.  
44. Show all active and inactive users from two tables using FULL OUTER JOIN.  
45. Display employee names and their direct reports using self JOIN and COUNT.  
46. Write a query to fetch all customers who have purchased items from more than one category using JOIN, GROUP BY, and HAVING.  
47. List all suppliers and the cities they operate in using JOIN and DISTINCT.  
48. Write a query to find the total salary expenses by department using JOIN and GROUP BY.  
49. Show all customers who made purchases in each quarter of 2024 using JOIN and date functions.  
50. Display employees whose salaries are above the average salary of all employees using JOIN and aggregation.

### GROUP BY and HAVING Exercises (51-100)

51. Write a query to display the total sales per country using GROUP BY.  
52. Find the number of employees in each department using GROUP BY.  
53. Display the average salary of employees grouped by job title using GROUP BY.  
54. Write a query to find all products where the total quantity sold is greater than 500 using HAVING.  
55. Find the departments which have more than 10 employees using GROUP BY and HAVING.  
56. Display the number of orders per customer and filter customers who have more than 5 orders using HAVING.  
57. Write a query to calculate the total commission earned per salesperson using GROUP BY.  
58. Find all cities where the average customer grade is greater than 200 using GROUP BY and HAVING.  
59. Display the maximum salary per department using GROUP BY.  
60. Write a query to find products with sales amount less than the average sales amount using HAVING.  
61. List all employees earning above the average salary within their department using GROUP BY, HAVING, and analytic functions.  
62. Find customers who have ordered all products from a specific category using GROUP BY and HAVING.  
63. Write a query to find salespersons who have sold products worth more than $100,000.  
64. Display the department names with total salary expense greater than $500,000 using GROUP BY and HAVING.  
65. List all job titles where fewer than 5 employees are working using GROUP BY and HAVING.  
66. Write a query to get the total number of orders, total quantity, and average price for each product category.  
67. Display the number of students enrolled in each course who scored above 75 using GROUP BY and HAVING.  
68. Find cities with more than 2 salespersons using GROUP BY and HAVING.  
69. Write a query to list all suppliers with total supplied quantity exceeding 1000 units using GROUP BY and HAVING.  
70. Display departments that do not have any employee earning below $3000 using HAVING.  
71. Write a query to identify customers who placed orders on all available order dates using GROUP BY and HAVING.  
72. Find products with average customer ratings greater than 4 using GROUP BY and HAVING.  
73. List all employees whose salary is equal to the maximum salary in their department using GROUP BY and HAVING.  
74. Write a query to calculate the total revenue generated each month and filter months where revenue was less than $10,000.  
75. Find the number of customers per city having more than 3 orders using GROUP BY and HAVING.  
76. Display all departments with the total number of employees and average salary using GROUP BY.  
77. List products that have been ordered more than 5 times in each region using GROUP BY and HAVING.  
78. Write a query to find the average number of days employees spend on a project grouped by project name.  
79. Show job titles which have a salary range (max-min) greater than $5000 using GROUP BY and HAVING.  
80. Find customers who have spent more than the average amount spent by all customers using GROUP BY and HAVING.  
81. Write a query to display products grouped by category and show only those categories where the total stock is less than 100.  
82. Find cities where total sales amount exceeds $1 million using GROUP BY and HAVING.  
83. Display employees grouped by manager and filter those managers who have more than 5 direct reports using HAVING.  
84. Find customers who placed orders only in the last quarter using GROUP BY and HAVING.  
85. Write a query to find the average salary of employees hired each year using GROUP BY.  
86. List departments with the highest average salary using GROUP BY and ORDER BY LIMIT.  
87. Find all suppliers whose products have an average price higher than $50 using GROUP BY and HAVING.  
88. Display customer IDs and count of distinct products ordered using GROUP BY and HAVING.  
89. Write a query to find the total sales per salesman and filter salesmen with sales greater than $50,000.  
90. Find the number of employees with same job title and salary grouped together using GROUP BY and HAVING.  
91. List all orders grouped by shipping company and filter those with total orders greater than 100.  
92. Write a query to get the total quantity ordered for each product and filter products ordered by at least 10 customers.  
93. Find all projects with the number of employees assigned and filter projects with less than 3 employees.  
94. Display cities and the average customer rating, filtering cities with average rating less than 3.5.  
95. Find job titles with minimum salary above $6000 using GROUP BY and HAVING.  
96. Write a query to group employees by country and count employees having salaries above $7000.  
97. Find customers whose orders have a total quantity greater than the average order quantity for all customers.  
98. List the total commission per department and show only departments with commissions above 10,000.  
99. Write a query to find months with the highest and lowest sales using GROUP BY and HAVING.  
100. Display salesmen who have closed deals with at least 3 different customers using GROUP BY and HAVING.




[1] https://www.w3resource.com/sql-exercises/sql-joins-exercises.php
[2] https://www.w3schools.com/sql/sql_join.asp
[3] https://datalemur.com/sql-tutorial/sql-joins-inner-outer-left-right
[4] https://learnsql.com/blog/sql-joins-practice/
[5] https://www.scribd.com/document/479067387/SQL-Exercises-HR-Database-JOINS
[6] https://www.codechef.com/practice/sql-case-studies-topic-wise
[7] https://www.wiseowl.co.uk/sql/exercises/standard/basic-joins/
[8] https://www.hackerrank.com/domains/sql/join/difficulty:true/page:1/
[9] https://www.w3schools.com/sql/exercise.asp?x=xrcise_join1
[10] https://datalemur.com/questions/sql-join-practice-exercise-robinhood


[1] https://www.linkedin.com/pulse/top-100-sql-interview-questions-answers-2025-paras-grover-hzqmf
[2] https://www.simplilearn.com/top-sql-interview-questions-and-answers-article
[3] https://www.datacamp.com/blog/top-sql-interview-questions-and-answers-for-beginners-and-intermediate-practitioners
[4] https://www.w3resource.com/sql-exercises/
[5] https://www.geeksforgeeks.org/sql/sql-interview-questions/
[6] https://www.geeksforgeeks.org/sql/sql-exercises/
[7] https://datalemur.com/sql-interview-questions
[8] https://www.codechef.com/practice/sql-case-studies-topic-wise
[9] https://datatrained.com/post/sql-practice-questions/
[10] https://techbeamers.com/sql-query-questions-answers-for-practice/
[11] https://dev.to/abhay_yt_52a8e72b213be229/100-essential-sql-questions-every-developer-should-master-3mop
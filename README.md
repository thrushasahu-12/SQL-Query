# SQL-Query
In this Repo i will be updating the Question and Answers of the SQL Practice

you can try writing SQL queries for the following:

Find all employees who work in the IT department.

List employees whose salary is greater than 100000.

Get employees who joined after '2020-01-01'.

Find employees who live in 'Ramseyhaven'.

Show employees with the position 'Analyst'.

List employees who are not in the HR department.

Find employees whose salary is between 100000 and 120000.

Get employees from the 'Sales' department who live in 'Lake Erichaven'.

List employees whose first name starts with 'R'.

Show employees who joined before 2019 and have salary less than 120000.

_____________________________________________________________________________________

-- SELECT all rows

SELECT * FROM [dbo].[employee-dataset];

-- SELECT unique departments

SELECT DISTINCT Department FROM [dbo].[employee-dataset];

-- Employees in IT department

SELECT * FROM [dbo].[employee-dataset]
WHERE Department = 'IT';

-- Employees with salary > 100000

SELECT * FROM [dbo].[employee-dataset]
WHERE Salary > 100000;

-- Employees joined after 2020

SELECT * FROM [dbo].[employee-dataset]
WHERE JoiningDate > '2020-01-01';

-- Employees in Ramseyhaven city

SELECT * FROM [dbo].[employee-dataset]
WHERE City = 'Ramseyhaven';

-- Employees with position Analyst

SELECT * FROM [dbo].[employee-dataset]
WHERE Position = 'Analyst';

-- Employees not in HR

SELECT * FROM [dbo].[employee-dataset]
WHERE Department != 'HR';

-- Employees with salary between 100000 and 120000

SELECT * FROM [dbo].[employee-dataset]
WHERE Salary BETWEEN 100000 AND 120000;

-- Employees in Sales department and Lake Erichaven

SELECT * FROM [dbo].[employee-dataset]
WHERE Department = 'Sales' AND City = 'Lake Erichaven';

-- Employees whose first name starts with 'R'

SELECT * FROM [dbo].[employee-dataset]
WHERE FirstName LIKE 'R%';

-- Employees joined before 2019 and salary < 120000

SELECT * FROM [dbo].[employee-dataset]
WHERE JoiningDate < '2019-01-01' AND Salary < 120000;



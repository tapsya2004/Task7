# Task7
/*CREATE TABLE Departments (
    dept_id INT PRIMARY KEY,
    dept_name VARCHAR(100)
);

CREATE TABLE Employees (
    emp_id INT PRIMARY KEY,
    emp_name VARCHAR(100),
    salary INT,
    dept_id INT,
    FOREIGN KEY (dept_id) REFERENCES Departments(dept_id)
);
INSERT INTO Departments (dept_id, dept_name) VALUES
(1, 'HR'),
(2, 'IT'),
(3, 'Finance');

INSERT INTO Employees (emp_id, emp_name, salary, dept_id) VALUES
(101, 'Amit', 55000, 1),
(102, 'Neha', 72000, 2),
(103, 'Ravi', 48000, 1),
(104, 'Meera', 69000, 3),
(105, 'Vijay', 61000, 2);
CREATE VIEW IT_Employees AS
SELECT emp_id, emp_name, salary
FROM Employees
WHERE dept_id = 2;
DROP VIEW IF EXISTS EmployeeDetails;

CREATE VIEW EmployeeDetails AS
SELECT 
    e.emp_id, 
    e.emp_name, 
    e.salary, 
    d.dept_name
FROM 
    Employees e
JOIN 
    Departments d ON e.dept_id = d.dept_id;
CREATE VIEW HighSalaryEmployees AS
SELECT * FROM Employees
WHERE salary > 60000
WITH CHECK OPTION;
SELECT * FROM IT_Employees;*/

SELECT * FROM EmployeeDetails
WHERE dept_name = 'Finance';







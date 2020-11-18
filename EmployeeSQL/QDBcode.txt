departments
-
dept_no VARCHAR PK
dept_name VARCHAR

dept_emp
-
emp_no INT FK >- employees.emp_no
dept_no VARCHAR FK >- departments.dept_no

dept_manager
-
dept_no VARCHAR FK >- departments.dept_no
emp_no INT FK >- employees.emp_no

employees
-
emp_no INT PK
emp_title VARCHAR
birth_date DATE
first_name VARCHAR
last_name VARCHAR
sex VARCHAR
hire_date DATE

salaries
-
emp_no INT FK >- employees.emp_no
salary INT

titles
-
emp_title VARCHAR FK  >- employees.emp_title
title VARCHAR

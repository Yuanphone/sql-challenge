# sql-challenge
### Employee Database
## Background
In this assignment, our first major task is a research project on employees of the corporation from the 1980s and 1990s. All that remains of the database of employees from that period are six CSV files. We will design the tables to hold data in the CSVs, import the CSVs into a SQL database, and answer questions about the data. In other words, we will perform data modeling, data engineering, and data analysis.
## Data Modeling
The ERD was generated by using http://www.quickdatabasediagrams.com. In the ERD model, the csvs files were inspected. See below:

<img width="483" alt="ERD_Employee" src="https://user-images.githubusercontent.com/100816322/168655611-e1af115e-56ba-4d5f-9625-7456ad0f5a7b.PNG">

## Data Engineering
Use the provided information to create a table schema for each of the six CSV files. Remember to specify data types, primary keys, foreign keys, and other constraints.
For the primary keys, verify that the column is unique. Otherwise, create a composite key, which takes two primary keys to uniquely identify a row.
Be sure to create tables in the correct order to handle foreign keys.
Import each CSV file into the corresponding SQL table.

## Data Analysis
After completing the database, perform the following steps:

List the following details of each employee: employee number, last name, first name, sex, and salary.

List first name, last name, and hire date for employees who were hired in 1986.

List the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name.

List the department of each employee with the following information: employee number, last name, first name, and department name.

List first name, last name, and sex for employees whose first name is "Hercules" and last names begin with "B."

List all employees in the Sales department, including their employee number, last name, first name, and department name.

List all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.

List the frequency count of employee last names (i.e., how many employees share each last name) in descending order.
## Bonus
To check if the dataset is fake, the visualization of the data was created.

### 1. Import the SQL database into Pandas.

### 2. Create a histogram to visualize the most common salary ranges for employees.
![salaryrange](https://user-images.githubusercontent.com/100816322/168657455-5efb5b2f-c153-4e6f-ac03-c7c5bfc685e5.png)

#### Anaysis: The most common salary range for employees is 40000 which has the highest frequency of 140000. 

### 3 Create a bar chart of average salary by title.
![salarybytitle](https://user-images.githubusercontent.com/100816322/168668521-7ce2fef6-b707-4dff-a564-57dad3cf8aea.png)

#### Analysis: From the bar chart, the salaries for assitant engineer, engineer and senior engineer are similar, and the salaries for staff and senior staff are also similar. This is unreseasonable. Usually, different levels of titles mean different salaries. Therefore, this dataset seems to be fake.

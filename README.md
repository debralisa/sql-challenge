# sql-challenge
##Background

It’s been two weeks since you were hired as a new data engineer at Pewlett Hackard (a fictional company). Your first major task is to do a research project about people whom the company employed during the 1980s and 1990s. All that remains of the employee database from that period are six CSV files.

###This Challenge is divided into three parts: data modeling, data engineering, and data analysis.


###DATA MODELING:  I reviewed the 6 csv files, reviewed what columns existed in each file, what were common key possiblities and from there began to create an Entity Relationship Diagram (ERD).  Starting out using QuickDBD to create an initial ERD (conceptual schemata), and as I inspected the columns and determined what would be best primary keys, created the logical schemata and finally added the remaining columns and included the data types (the physical schemata).  Once I was satisfied with the best schemata, I used QuickDBD export feature to save the ERD to a png file.

###Data Engineering

I also used the export feature in QuickDBD from my physical schemata to save to a PostgreSQL file.  I cleaned up and ran the table schema for each of the 6 CSV files in pgAdmin in the Employee SQL Database that I had created.  As suggested in the HINT for the assignment, I made sure that I created the tables in the correct order to handle the foreign keys.  Once the tables were created, I loaded the data files into each table, also in the order that the tables were created.

###Data Analysis

I created a query file to answer the following 8 queries:

#1-List the employee number, last name, first name, sex, and salary of each employee.
#2-List the first name, last name, and hire date for the employees who were hired in 1986.
#3-List the manager of each department along with their department number, department name, employee number, last name, and first name.
#4-List the department number for each employee along with that employee’s employee number, last name, first name, and department name.
#5-have List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.
#6-List each employee in the Sales department, including their employee number, last name, and first name.
#7-List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.
#8-List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).

###File Names/Folder Names

#EmployeeSQL folder containing: employee_schemata.sql (table schemata file), employeeERD.png (ERD diagram), employeequery.sql (query file for the 8 queries), data folder containing the 6 csv files for the corresponding tables.

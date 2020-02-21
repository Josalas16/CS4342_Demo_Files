<h1 align="center">
  <br>
  <img src="https://www.utep.edu/Images/utep%20logo.png" alt="UTEP logo" width="200">
  <br>
  CS 4342 Database Management Starter Code
  <br>
</h1>

Template PHP files to be used by the CS4342 students at the University of Texas at El Paso during the Spring 2020 semester. These files will provide the structure and knowledge on how to validate information from a database as well as the concepts of data insertion, through a web interface using PHP.

---
## Config File
Here you will find the configuration settings for the database connections. You need to change the following lines for your setup:
- *host* (line 10) this should be the utep ilinkserver. 
- *db* (line 11) this should be the database name for your team. It should be named `s20x_teamY`.
- *username* (line 13) this should be the utep username of the person who volunteers from your team.
- *password* (line 14) this should be a password agreed upon by your team so that your team can make necessary changes. This password is the same that your teammate from above uses to login and interact with mySQL shell.

---
## Create Account
Here you will see a template form that takes in user input and inserts it into the database. For this to work you **MUSt** have created the Student table beforehand. Your student table can be created as follows:

```SQL
CREATE TABLE Student (U_username VARCHAR(20), U_password VARCHAR(10), U_first VARCHAR (20), U_middle VARCHAR(20), U_last VARCHAR(20));
```
---
## Student Login
Here you will see a template form that validates user login information that has been entered into the database. For this to work you **MUST** have created the Student table beforehand, as well as have some information stored there from which the 
comparisons can be made in order to successfully login or throw a message if no user was found. An example of how to insert data into this table is provided below:

```SQL
INSERT INTO Student VALUES ('student1','myPswd','John','A','Smith');
```

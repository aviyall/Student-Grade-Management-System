# Student Grade Management System

This is a simple Student Grade Management System built using Python and MySQL. The system allows you to manage student information, grades, and calculate percentages.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Demo](#demo)
- [Features](#features)
- [Contributing](#contributing)

## Prerequisites

Before running this application, ensure you have the following installed:

1. **Python 3.x**: Download and install from [Python's official website](https://www.python.org/downloads/).
2. **MySQL Server**: Download and install MySQL from [MySQL's official website](https://dev.mysql.com/downloads/mysql/).

## Installation

1. **Install MySQL Server**:
   - Follow the instructions to install MySQL.
   - During the installation, set up a root password (default is often blank).

2. **Install pip** (Python package manager):
   - If you have Python installed, `pip` should already be available. You can check by running:
     ```bash
     pip --version
     ```

3. **Install mysql-connector-python**:
   - Open your terminal or command prompt and run:
     ```bash
     pip install mysql-connector-python
     ```

## Usage

1. **Create a Database**:
   - After installing MySQL, open the MySQL command line or a MySQL GUI tool (like MySQL Workbench) and create a database:
     ```sql
     CREATE DATABASE Class1; -- Replace '1' with your class number
     ```

2. **Run the Application**:
   - Download or clone this repository.
   - Navigate to the project directory in your terminal or command prompt and run:
     ```bash
     python your_script_name.py
     ```

## Demo

### Establishing a Basic Connection Using mysql.connector

Here’s a brief demo of how to establish a connection to your MySQL database using the `mysql.connector` module:

```python
import mysql.connector

# Establish a connection
conn = mysql.connector.connect(
    host='localhost',
    user='root',
    password='your_password'  # Replace with your MySQL root password
)

# Check if the connection was successful
if conn.is_connected():
    print("Successfully connected to the database!")
else:
    print("Failed to connect to the database.")

# Close the connection
conn.close()
```
## Run the Main code

### OUTPUT:
```text
Student Grade Management System
SELECT A CLASS DATABASE
1. class10
2. class11
3. class12
4. Create new database
5. Exit
Enter your choice (1-5):3
```
Selects Class12;
```text
Student Grade Management System
1. Add student and grades
2. View grades by student name
3. Calculate percentage for a student
4. List all students with their ranks
5. Exit
Enter your choice (1-5):
```
Main menu is displayed;
```text
Student Grade Management System
1. Add student and grades
2. View grades by student name
3. Calculate percentage for a student
4. List all students with their ranks
5. Exit
Enter your choice (1-5): 1
Enter student name: Rahul Rajesh
Enter maximum marks for all subjects: 100
Enter grade for Physics: 94
Enter grade for Chemistry: 92
Enter grade for Mathematics: 89
Student Rahul Rajesh and their grades have been added.

Press Enter to continue...
```
Student detail added;
```text
Student Grade Management System
1. Add student and grades
2. View grades by student name
3. Calculate percentage for a student
4. List all students with their ranks
5. Exit
Enter your choice (1-5): 4
List of all students with their ranks:
Rank: 1, Name: Devika, Percentage: 96.67%
Rank: 2, Name: Rahul Rajesh, Percentage: 91.67%
Rank: 3, Name: Prakash Wilson, Percentage: 82.00%

Press Enter to continue...
```
Listing added students rank wise;
```text
Student Grade Management System
1. Add student and grades
2. View grades by student name
3. Calculate percentage for a student
4. List all students with their ranks
5. Exit
Enter your choice (1-5): 5
Exiting the system.
```
Exiting:


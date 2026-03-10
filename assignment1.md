# Assignment 1 You meant to design. And bring out insights from a school db
Student table 
Fields:
Name 
Email
Student ID 
Schoolname

Exam table
Coursename
CourseID
Exam mark 
Student ID 
Staff Id

Payment table 
Amount paid
Bank name
Account name
Student ID 
Payment date

# Question:

# Pls write an SQL query pulling The following records
# Name, email, amount paid, payment date, student ID 

# solution
SELECT Name, email, amount paid, payment date, student ID FROM student
INNER JOIN Payment on student.student ID = Payment.student ID

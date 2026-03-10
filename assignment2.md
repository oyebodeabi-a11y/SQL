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

# Write an SQL queries pulling the following records 
Course Id, course name,student ID,name,email ,staffId

# Solution
Select courseID, Coursename, student ID, name, email, StaffID FROM Exam
INNER JOIN Student on student.student ID = email.student ID
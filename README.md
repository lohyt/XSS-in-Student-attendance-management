# XSS-in-Student-attendance-management

Description: Persistent Cross Site Scripting found in Student Attendance Management System from Sourcecodester website.

[Additional Information] NA

[Vulnerability Type] Cross Site Scripting (XSS)

[Vendor of Product] https://www.sourcecodester.com/

[Affected Product Code Base] Student Attendance Management System

[Affected Component] http://localhost/student_attendance/index.php?page=courses

[Attack Type] Remote

[Impact Information Disclosure] true

[Attack Vectors] Steps to reproduce:
Go to url http://localhost/student_attendance/
Click on "Course" in the left column
Enter the payload "<img(space)src=1(space)href=1(space)onerror="javascript:alert(1)">" in the "Course" field (PS: Replace (space) with regular space)
Click on "Save"
XSS will be triggered and pop up appears.


[Discoverer] M Lohith

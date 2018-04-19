
WorkingWithMongoDB:
The database of a company is depicted in JSON format using Mongo DB and two schemas have been created as:

    1.	The PROJECT document will include the following data: Pnumber, Pname, Dname (of the controlling department), plus a list of the employees that work on the project {employees: Lname, Fname, Hours}.

    2.	The DEPARTMENT document will include the following data: Dname, the department manager’s Lname, and a list of the locations of the department {locations: Dlocation}

Data Structures Used:
•	Programming Language: Python
•	Python Dictionary: to create JSON object 
•	List: For list of Employees and Department in the dictionary


Steps To Follow:
1.	Perform SQL database connection
2.	Load Data for all tables in SQL
3.	Create MongoDB database
4.	Create two Collections 'Projects_Collection' and 'Departments_Collection'
5.	Write SQL query for Projects Collections by joining Employee, Department, Projects and WorkOn Tables and fetch the required columns from each of the tables as follows:
PNumber, Pname,Dname,Fname,Lname,Hours
6.	Execute the above query and fetch all the rows of results in a variable project_result
7.	Create a python dictionary project_document = {}
8.	Map the results that is stored in the project_result and create a json object or document by creating a dictionary where PNumber will be Key 
9.	Insert the created dictionary in project collection document

10.	Write SQL query for Department Collections by joining Employee, Department, Dept_Locations Tables and fetch the required columns from each of the tables as follows:
Dname,Lname,Dept_Locations
11.	Execute the above query and fetch all the rows of results in a variable department_result
12.	Create a python dictionary department_document = {}
13.	Map the results that is stored in the department _result and create a json object or document by creating a dictionary where DName will be Key 
14.	Insert the created dictionary in departments collection document

15.	Print both the collections and the documents


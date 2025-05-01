<h1> Employee Data Segmentation and Analysis System </h1>

<h2>Description</h2>
This project implements a structured relational database system to organize, segment, and analyze employee data based on work location and data sensitivity. By creating and populating normalized tables, the solution facilitates efficient data management, enables logical data separation (e.g., frequently vs. infrequently accessed data), and supports insightful queries that drive informed HR and operational decisions.
<br />

<h2>Languages and Utilities Used</h2>

- <b> SQL </b> 

<h2>Environments Used </h2>

- <b> Microsoft SQL Server Management Studio </b>

<h2>Project walk-through:</h2>

<p align="left">
The SQL query creates the Employeetable to store employee details, including ID, name, gender, <br/> phone, date of birth, and work location, with each field defined as varchar(50). <br/><br/>
  <img src="Screenshot 2025-04-30 211835.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
 This query inserts multiple employee records into the EmployeeTable, including details like ID, <br/> name, gender, phone number, date of birth, and work location. <br/><br/>
  <img src="Screenshot 2025-04-30 211850.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query retrieves all columns and records from the `Employeetable`, displaying the details of<br/> every employee stored in the table. <br/><br/>
  <img src="Screenshot 2025-04-30 211900.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
 This query creates a table named Denver_Employee with columns for employee details, including ID,<br/> name, gender, phone number, date of birth, and work location, all defined as <br/> VARCHAR(50) to store text-based information. <br/><br/>
  <img src="Screenshot 2025-04-30 211916.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query creates a table named `Phoenix_Employees` with columns to store employee information, <br/> including ID, name, gender, phone number, date of birth, and work location, all <br/> defined as `VARCHAR(50)` to accommodate text-based data. <br/><br/>
  <img src="Screenshot 2025-04-30 211923.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
 This query inserts records into the `Denver_Employee` table by selecting all columns from the  <br/> `Employeetable` where the `EmpWorkLocation` is 'Denver', effectively copying the  <br/> employee data for those located in Denver into the new table. <br/><br/>
  <img src="Screenshot 2025-04-30 212037.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query inserts records into the `Phoenix_Employees` table by selecting all columns from the <br/> `Employeetable` where the `EmpWorkLocation` is 'Phoenix', copying the employee data <br/> for those located in Phoenix into the new table. <br/><br/>
  <img src="Screenshot 2025-04-30 212057.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query retrieves all columns and records from the Phoenix_Employees table, displaying the <br/> details of all employees stored in that table. <br/><br/>
  <img src="Screenshot 2025-04-30 212114.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
 This query retrieves all columns and records from the `Denver_Employee` table, displaying the  <br/> details of all employees stored in that table. <br/><br/>
  <img src="Screenshot 2025-04-30 212120.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query combines the results from the `Denver_Employee` and `Phoenix_Employees` tables, <br/> retrieving all unique records from both tables. The `UNION` operator ensures that duplicate <br/>  rows are excluded from the result set. <br/><br/>
  <img src="Screenshot 2025-04-30 212127.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query creates a table named `Employee_Frequent` with columns for employee ID, name, and <br/> work location; the `EmpID` column is set as the primary key to uniquely identify each record. <br/><br/>
  <img src="Screenshot 2025-04-30 212133.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query inserts employee ID, name, and work location data from the `EmployeeTable` into the <br/> `Employee_Frequent` table. <br/><br/>
  <img src="Screenshot 2025-04-30 212138.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query creates a table named `Employee_NotFrequent` to store less frequently accessed employee <br/> details, including gender, phone number, and date of birth, with `EmpID` as the <br/> primary key. <br/><br/>
  <img src="Screenshot 2025-04-30 212144.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query inserts employee ID, gender, phone number, and date of birth from the `Employeetable`  <br/> into the `Employee_NotFrequent` table. <br/><br/>
  <img src="Screenshot 2025-04-30 212150.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This query retrieves all records from the `Employee_NotFrequent` table, displaying essential employee <br/> details such as ID, gender, phone number, and date of birth. <br/><br/>
  <img src="Screenshot 2025-04-30 212159.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>

<p align="left">
This SQL query joins the `Employee_NotFrequent` and `Employee_Frequent` tables on the `EmpID` column,  <br/> returning only the employee records present in both tables, including demographic  <br/> and location details. <br/><br/>
  <img src="Screenshot 2025-04-30 212207.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
</p>
```

This code will display each screenshot in the specified order with a title for each and an image size of 80% of the container width and height.

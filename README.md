# Simple SQL attack simulation and analysis


## Objective
The main objective is to create a basic mysql server and create a login web page which checks the content in the mysql server (like username and password) and perform a sql injection attack. Then analize the evidences using autopsy and create a disk image to preserve evidences using FTK imager.


### Skills Learned
- Using XAMPP to create a mysql and apache server on our localhost
- creating a basic login html and a php file
- Basics of sql injection attakcs ( about malicious inputs)
- Basics of autospy -analyzing a basic evidence_log file
- basics of FTK imager -creating a image file

### Tools Used

- XAMPP -to create a mysql and a apache server on localhost
- autopsy -to analyze the evidences
- FTK imager -to create an image file

## XAMPP
<img src="https://img.shields.io/badge/XAMPP-FF7A00?style=for-the-badge&logo=xampp&logoColor=white" />

XAMPP is a free software that lets you run a web server on your own computer
- X  -Cross-platform (works on Windows, Linux, Mac)
- A  -Apache (web server)
- M  -MySQL / MariaDB (database)
- P  -PHP (programming language)
- P  -Perl (programming language)

## Autospy
<img src="https://img.shields.io/badge/Autopsy-Digital_Forensics-blue?style=for-the-badge" />

Autopsy is a digital forensics tool used to analyze computers, hard drives, and files to find evidence
It is used to,
- Recover deleted files
- Analyze hard disks 
- Check browser history 
- Find hidden or suspicious files 
- Detect malware activity 

## FTK imager
<img src="https://img.shields.io/badge/FTK%20Imager-Forensics-4B0082?style=for-the-badge&logo=windows&logoColor=white"/>

FTK Imager is a tool used to copy and examine data from a computer or hard drive for investigation purposes

## Steps

### Step 1 -Configure apache and mysql server using XAMPP
<img width="1920" height="1040" alt="configuring the localhost server by starting apache" src="https://github.com/user-attachments/assets/49cacadb-c62d-4e82-8b70-df0ddce954dc" />


### Step 2-Create a database and add values to the table
<img width="1920" height="1039" alt="creating hope hospital database" src="https://github.com/user-attachments/assets/a851d5b2-2281-4ef7-bb77-0e22f620c13f" />
<img width="1920" height="1038" alt="creating tables1" src="https://github.com/user-attachments/assets/1ffb9007-86fb-470a-a2ae-4b35505df7de" />
<img width="1920" height="1039" alt="table2" src="https://github.com/user-attachments/assets/09dea470-b4dc-4fe5-b852-21fa76fe9bf7" />


### Step 3-Create login html (login page)
<img width="1920" height="1080" alt="loginhtml" src="https://github.com/user-attachments/assets/6a76d9a5-ba74-4148-9f26-a0510f76998f" />


### step 4-Create login php
<img width="1422" height="1023" alt="loginphp" src="https://github.com/user-attachments/assets/f44c687b-ebf8-49e1-9459-6e37deda94d7" />

- php file is used to connect the database and check whether the login details are correct

### Step 5-Admin login
<img width="1920" height="1039" alt="adminlogin" src="https://github.com/user-attachments/assets/44dae0d2-73c0-4737-bd98-50d2e6c6c205" />
<img width="1920" height="1042" alt="adminlogin2" src="https://github.com/user-attachments/assets/ab5fe5eb-161c-420a-8110-e130ca4b6e53" />

### Step 6-User login
<img width="1920" height="1036" alt="userlogin" src="https://github.com/user-attachments/assets/5f93f93f-efcd-4f27-8851-1310b7c14fb2" />
<img width="1920" height="1040" alt="userlogin2" src="https://github.com/user-attachments/assets/4d87117b-4374-4d59-97c8-c9fa02876c46" />

### Step 7-SQL injection 
<img width="1920" height="1040" alt="sqlworkinginjec" src="https://github.com/user-attachments/assets/3ebeff24-adb5-4b08-b974-f4e1c96ef3a1" />

<img width="1920" height="1039" alt="sqlworkinginjec2" src="https://github.com/user-attachments/assets/9a8ae683-8c05-4834-b029-d61a0753edc6" />
 
SQL injection happens when an application:

- takes user input,
- puts it directly into an SQL query,
- and does not properly separate data from code.

Because of that, the database may treat part of the user’s input as SQL commands instead of plain text.
At a conceptual level, that input tries to do three things:

- ' -closes the text value the app was expecting
- OR 1=1 -adds a condition that is always true
- '#'-comments out the rest of the query in some SQL dialects

So instead of the app checking “does this exact username and password match?”, the query logic can get changed into something like:

“username matches or this always-true condition is true”

### step 8-Use autopsy to analyze evidence

- Adding the data source
<img width="1699" height="919" alt="adding thedatasource1" src="https://github.com/user-attachments/assets/5fadaa73-2e85-4437-8926-dc5e01dfbc3d" />

- Adding case details
<img width="1704" height="904" alt="autospsy case1" src="https://github.com/user-attachments/assets/60ea7967-6ef5-4cf3-ad9d-35cf29e6af98" />

- Inspecting evidence
<img width="1704" height="906" alt="inspecting evidence" src="https://github.com/user-attachments/assets/020ce0e8-4443-4763-83ce-56210180dcd2" />

- At 10.30 AM there was a login attempt using the username admin
- At 10.32 AM there was a suspicious login attempt ( ' OR 1 = 1 #)
- At 10.33 AM access granted to the system
- AT 10.35 patient records viewed

We can gather valuable information like evidence logs using web servers, sql servers etc. Most of the time, activities in a server recorded as log files.

### step 9-Use FTK imager to image the affected file.

- selecting the source file
<img width="1920" height="1080" alt="selecting the source file" src="https://github.com/user-attachments/assets/13b6a9e9-7975-4dbd-a70e-29dfd87a65a0" />

- adding details of the case

Adding details like case information, case id, evidence number, examiner etc is important in digital forensics.
<img width="1920" height="1080" alt="details of he case" src="https://github.com/user-attachments/assets/88179a6e-a01b-401c-afd7-8d0e155b321b" />


- Confirmation
<img width="1920" height="1080" alt="progress of the imaging" src="https://github.com/user-attachments/assets/d06c1905-60ee-4167-a292-9bdcea09a2c1" />
<img width="1920" height="1080" alt="confirmation" src="https://github.com/user-attachments/assets/b8015071-5404-440c-a95d-baf4438cc82b" />

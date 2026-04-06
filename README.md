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

- 



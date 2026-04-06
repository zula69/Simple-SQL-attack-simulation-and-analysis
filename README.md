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


### Step 3-Enumerate the Target
![nmap](https://github.com/user-attachments/assets/2ed55376-7f11-4988-a2d3-ceaf85a3a087)

### step 4-Exploit Telnet
![telnet](https://github.com/user-attachments/assets/e91f25dd-4ba6-473f-a580-eaf8e65274bc)
![telnet2](https://github.com/user-attachments/assets/4ea2ef91-993b-46ff-b7bc-fc5dd8623a7b)
- someimes, due to the configuration mistakes, some important accounts can be left with blanks passwords. So we can try some typical names such as admin, root, administrator etc.


### Step 5-Capture the flag
![flag](https://github.com/user-attachments/assets/2cd94e9f-299e-40ea-abc4-275d8329506a)




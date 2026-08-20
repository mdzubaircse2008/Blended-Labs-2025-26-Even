# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: Mohammed Zubair R
* **Register Number**: 212225040252
* **Date of Submission**:20/08/2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)
First, a security group named DB Security Group was created to allow the web server to connect to the database using port 3306 (MySQL).


A DB Subnet Group was created with subnets from two Availability Zones to allow the database to run in a Multi-AZ environment for high availability.


A MySQL RDS instance named lab-db was created with the database name lab, username main, and password lab-password.


The database was associated with the DB Security Group and the Lab VPC so that the web server can securely connect to the database.


The web application running on the EC2 server was opened using its IP address, and the RDS endpoint, database name, username, and password were entered to interact with the database.


---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

<img width="1913" height="867" alt="image" src="https://github.com/user-attachments/assets/a8f0c677-2d8e-406b-a838-9ece3f8f413c" />



---

### Screenshot 2: Database Service Running

<img width="1912" height="870" alt="image" src="https://github.com/user-attachments/assets/712980a2-075e-4b7a-a98c-d5b3de9fd7bb" />



---

### Screenshot 3: Sample Database and Table

<img width="1912" height="906" alt="image" src="https://github.com/user-attachments/assets/577aec0f-4562-491b-b056-05d2ca7ea03b" />


---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst

# Data Leakage Detection

## Project Overview

Data Leakage Detection is a Java-based application developed using NetBeans IDE and Swing. It provides a secure file transfer protocol and integrates with a MySQL database (via XAMPP server) to manage user data, file information, and file transfers. The application also includes an admin role with full control over user activities, including monitoring file transfers and detecting potential data leaks.

## Prerequisites

Before setting up the project, ensure the following prerequisites are met:

1. **Install XAMPP Server with MySQL**:
   - Download and install XAMPP from [Apache Friends](https://www.apachefriends.org/index.html).
   - Start the XAMPP control panel and ensure MySQL is running.

2. **Create the Necessary Tables in MySQL**:
   Use the following SQL commands to create the required tables:
   ```sql
   CREATE TABLE emp (
     id INT AUTO_INCREMENT PRIMARY KEY,
     username VARCHAR(255) NOT NULL,
     password VARCHAR(255) NOT NULL
   );

   CREATE TABLE filedata (
     id INT AUTO_INCREMENT PRIMARY KEY,
     filename VARCHAR(255) NOT NULL,
     file_size BIGINT NOT NULL
   );

   CREATE TABLE filetransfer (
     id INT AUTO_INCREMENT PRIMARY KEY,
     sender_id INT NOT NULL,
     receiver_id INT NOT NULL,
     file_id INT NOT NULL,
     transfer_date DATETIME DEFAULT CURRENT_TIMESTAMP
   );

   CREATE TABLE fileid (
     id INT AUTO_INCREMENT PRIMARY KEY,
     file_reference VARCHAR(255) NOT NULL
   );

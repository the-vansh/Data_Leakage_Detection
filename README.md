# Data Leakage Detection

## Project Overview

Data Leakage Detection is a Java-based application developed using NetBeans IDE and Swing for creating a file transfer protocol. The project utilizes a MySQL database, specifically from XAMPP server, for storing information about users, files, and file transfers. The main functionality of the application allows users to securely send files to each other, requiring a passkey for file downloads. The project includes an admin role with complete control over user activities, monitoring file transfers, and detecting potential data leaks.

## Prerequisites

Before setting up the project, ensure the following prerequisites are met:

1. Install XAMPP server with MySQL.
2. Create the necessary tables in the MySQL database:
   - `emp`: User information table.
   - `filedata`: File information table.
   - `Receivefile`: Inforamtion of received file.
   - `Sendfile`:Inforamtion of sent file

## Libraries Used

The project relies on the following libraries:

- **MySQL Connector**: Used to establish a connection between the Java application and the MySQL database.

- **jBCrypt-0.4**: Utilized for password encryption and decryption.

## Setting Up the Project

Follow these steps to set up and run the project:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/the-vansh/Data_Leakage_Detection.git

2. **Open in NetBeans IDE**

1. Open NetBeans IDE.
2. Import the project.

3. **Configure MySQL Database**

1. Start XAMPP server and ensure MySQL is running.
2. Create the required tables (`emp`, `filedata`, `Receivefile`, `Sendfile`) in the MySQL database.

### Add Libraries

1. Add the MySQL Connector JAR to the project.
2. Add the jBCrypt-0.4 JAR to the project.

### Build and Run

1.src/dlp DLP.java

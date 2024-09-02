# Data Leakage Detection

## Project Overview

Data Leakage Detection is a Java-based application developed using NetBeans IDE and Swing for creating a file transfer protocol. The project utilizes a MySQL database, specifically from XAMPP server, for storing information about users, files, and file transfers. The main functionality of the application allows users to securely send files to each other, requiring a passkey for file downloads. The project includes an admin role with complete control over user activities, monitoring file transfers, and detecting potential data leaks.

## Prerequisites

Before setting up the project, ensure the following prerequisites are met:

1. Install XAMPP server with MySQL.
2. Create the necessary tables in the MySQL database:
   - `emp`: User information table.
   - `filedata`: File information table.
   - `filetransfer`: File transfer information table.
   - `fileid`: File ID table.

## Libraries Used

The project relies on the following libraries:

- **MySQL Connector**: Used to establish a connection between the Java application and the MySQL database.

- **jBCrypt-0.4**: Utilized for password encryption and decryption.

## Setting Up the Project

Follow these steps to set up and run the project:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/the-vansh/Data_Leakage_Detection.git

# Full-Stac-app
Full-Stack Application with MySQL Database [Backend JavaScript] [Frontend html, css. Jav]
This guide walks you through setting up a full-stack web application on Windows with a MySQL database, Node.js/Express backend, and an HTML/JavaScript frontend for inserting and fetching data through a locally hosted web portal.
Prerequisites
•	Node.js (v14 or later): Download and install from nodejs.org.
•	MySQL: Install MySQL Community Server from mysql.com. Choose the "Developer Default" setup type during installation.
 Initialize the Project
1.	Create a project directory:
2.	mkdir fullstack-app
3.	cd fullstack-app
4.	Initialize a Node.js project:
5.	npm init -y
****Install Backend Dependencies*****
Install Express, MySQL driver, and CORS:
npm install express mysql2 cors
****Set Up MySQL Database*****
1.	Start the MySQL service:
o	Open the MySQL Installer on Windows, select "MySQL Server," and ensure it’s running. Alternatively, start it via the Services app (search for "Services" in Windows, find "MySQL80" or similar, and start it).
2.	Log in to MySQL using MySQL Command Line Client or MySQL Workbench:
3.	mysql -u root -p
Enter the password you set during MySQL installation.
4.	Create a database and table:
5.	CREATE DATABASE fullstack_db;
6.	USE fullstack_db;
7.	CREATE TABLE users (
8.	    id INT AUTO_INCREMENT PRIMARY KEY,
9.	    name VARCHAR(255) NOT NULL,
10.	    email VARCHAR(255) NOT NULL
11.	);

******Create Backend Server*****
Create server.js in the fullstack-app directory:
*********Set Up the Frontend*******
1 Create Frontend Files
Create a public folder in the fullstack-app directory:
mkdir public
1.	Create public/index.html
2.  Create public/script.js:
********Run the Application********
1.	Ensure MySQL is running:
2.	Open the Services app (search "Services" in Windows), find "MySQL80" (or similar), and ensure it’s running.
3.	Start the backend server:
4.	cd fullstack-app
5.	node server.js
6.	Open your browser and navigate to http://localhost:3001.


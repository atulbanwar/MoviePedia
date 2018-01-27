# MoviePedia

__Duration__: Nov 2017 - Dec 2017

__Description__: MoviePedia is a web application which helps to search for a movie using combinations of multiple search criteria. Being the part of Applied Database course it demands the use of large dataset, database normalization, and use of database concepts like joins, subqueries, dynamic queries, procedures, triggers, and indexes. In order to fetch and display records in chunks, pagination was implemented using procedures.

__Course__: Applied Database (Fall 2016)

__Technologies__: AngularJS, Bootstrap, PHP and MySQL

__Role__: Software Developer

__Responsibilities__:

 - To prepare a big data set having at least 1 million rows.
 - Normalization of the database to 3NF.
 - Implementation of the user interface.
 - Implementation of procedures, dynamic queries, triggers, indexes to data retrieval as per search criteria.

__Instructions__:

 - Create database 'employee'
 - Execute following create table query:
	 ```MySQL
	 CREATE TABLE emp_details (  
		emp_id 		int(255) 		NOT NULL	AUTO_INCREMENT,
		emp_name 	varchar(255) 	NOT NULL,
		emp_email 	varchar(255) 	NOT NULL,
		emp_gender 	varchar(255) 	NOT NULL,
		emp_address 	varchar(255) 	NOT NULL,
		PRIMARY KEY (emp_id)
	);
	```
  
  - Edit datbase_connection from DatabaseFiles folder to as follow
  
	`$con = mysqli_connect("localhost", _username_, _password_, "employee"); /*employee is database name`

- Go to C:/wamp(64) folder/alias
- Create test.conf file (you can give any name)
- Copy paste following line into the test.conf file
	```
	Alias / "_path_of_project_root_/" 
	<Directory "_path_of_project_root_/">
		Options Indexes FollowSymLinks
		AllowOverride all
		<IfDefine APACHE24>
			Require local
		</IfDefine>
		<IfDefine !APACHE24>
			Order Deny, Allow
			Deny from all
			Allow from localhost ::1 127.0.0.1
		</IfDefine>
	</Directory>
	```
- Start wamp server
- Hit localhost from web browser

__Contributors__: Atul Banwar, Sanket Patil, Sharath Chandrika Mummoju

# MoviePedia - Applied Database Project | Framework: HTML-AngularJS-PHP-MYSQL

Instructions:
- Create database employee
- Execute following Create table query :
  CREATE TABLE emp_details (
emp_id int(255) NOT NULL AUTO_INCREMENT,
emp_name varchar(255) NOT NULL,
emp_email varchar(255) NOT NULL,
emp_gender varchar(255) NOT NULL,
emp_address varchar(255) NOT NULL,
PRIMARY KEY (emp_id)
);
- Edit datbase_connection from DatabaseFiles folder to as follow
  $con = mysqli_connect("localhost", _username_, _password_, "employee");  /*employee is database name
- Go to C:/wamp(64) folder/alias
- Create test.conf file (you can give any name)
- Copy paste following line into the test.conf file
Alias / "_path_of_project_root_/" 
<Directory "_path_of_project_root_/">
   Options Indexes FollowSymLinks
    AllowOverride all
  <IfDefine APACHE24>
    Require local
  </IfDefine>
  <IfDefine !APACHE24>
    Order Deny,Allow
	  Deny from all
	  Allow from localhost ::1 127.0.0.1
	</IfDefine>
</Directory>
- Start wamp server
- Hit localhost from web browser

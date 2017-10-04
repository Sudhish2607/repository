# repository
Integrated Learning Management System (ILMS)
	Project Title: Integrated Learning Management System (ILMS)
	Author: Sudhish Surendran Thazhakasseril


Steps to run this Project...(ILMS)

Softwares Required
1... Apache Tomcat-8 -- to be used as webserver with port 8081
2... Java  - jdk1.7.0_02
3... Oracle Database 10g Express Edition -- to be used as DB server with port 8080



Setup Instructions
1... Install Oracle Database 10g. Now to start the server, go to the bin directory of the oracle 10g installation software.
C:\oraclexe\app\oracle\product\10.2.0\server\BIN
and run StartDB.bat
Check whether the installation is done properly by hitting on the link http://localhost:8080/. If the installation is fine, then the url will open with License Agreement.
Now to create all the tables in DB, create a user by named "mcaproject" and password as "sudhish". Now run all the queries present in the Project directory of the CD to create all the table and insert few of the records in the table for testing.

2... Install Apache Tomcat 8. We are using port as 8081, since the default port 8080 is being utilized by the db server. If you have installed the software using Apache software provided in the CD, then no need to change the port, since I have already altered the port of the provided software.
Now to start the server, go to the bin directory of apache tomcat 8 installation software.
C:\Program Files (x86)\Apache Software Foundation\apache-tomcat-8.0.35\bin
and run startup.bat
Check whether the installation is done properly by hitting on the link http://localhost:8081/. If the installation is fine, then the url will open with Oracle webserver console.

3... Set a username and password for installation of this projects war file. For that go to the conf directory of the tomcat you have installed.
C:\Program Files (x86)\Apache Software Foundation\apache-tomcat-8.0.35\conf
Open the file tomcat-users.xml in notepad and paste below 2 lines in the file and save it.
<role rolename="manager-gui"/>
<user username="sudhish" password="sudhish" roles="manager-gui"/>

4... To install DLMS.war file of this project, go to below link
http://localhost:8081/
Now click on Manager App button on top right corner of the screen. Enter username as "sudhish" and password as ="sudhish" to login into the server.
Now go down to Deploy block and upload the DLMS.war file present in the Project directory of the CD then deploy the application.

5... To run the application hit the below url:
http://localhost:8081/DLMS/index.jsp

6... Sample users created in the project:
username and password for Admin:
Admin/Sudhish

username and password for Professor:
Sudhish/Sudhish

username and password for Student:
Sido/Sudhish

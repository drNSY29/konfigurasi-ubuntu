# Mariadb Service
* Install mariadb service
``````
apt install mariadb-server -y
``````
* Start and enable mariadb-server
``````
systemctl enable --now mariadb-server
``````
* Initial setup mariadb
``````
mysql_secure_installation
``````
* Connect to console mariadb
``````
mysql -u root -p
``````
* Show User list in database
``````
MariaDB [(none)]> select user,host,password from mysql.user; 
``````
* Creating user
``````
 MariaDB [(none)]> create user test1 identified by 'password';
``````
* Give roles or permission to user
``````
MariaDB [(none)]> grant all on *.* to test1;
``````
* Flush privileges after give permission
``````
MariaDB [(none)]> flush privileges;
``````
* Show database in host
``````
MariaDB [(none)]> show databases; 
``````
* Create database test
``````
MariaDB [(none)]> create database test_database;
``````
* Create table in database test with schema
``````
MariaDB [(none)]> create table test_database.test_table (No int, Nama varchar(50), Alamat varchar(50), primary key (No)); 
``````
* Insert the data to the tables
``````
MariaDB [(none)]> insert into test_database.test_table(No, Nama, Alamat) values("01", "Zakaria", "Jakarta"); 
``````
* View data in tables
``````
MariaDB [(none)]> select * from test_database.test_table; 
``````

* Delete the database
``````
MariaDB [(none)]> drop database test_database; 
``````

* Exit
``````
MariaDB [(none)]> exit;
``````

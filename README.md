# BlogHole
Story/blog management system using flask

Install the following packages:
1. Flask
2. flask_mysqldb
3. wtforms
4. passlib
5. functools

Create your own mysql database named flaskdb with user as 'root' and password as '12345678'.
Run the following commands in your mysql console:

grant all privileges on *.* to root@localhost identified by '12345678' with grant option;
use flaskdb;
create table users (
`name` varchar(100),
`email` varchar(100),
`username` varchar(100),
`password` varchar(100),
primary key(`username`));
create table articles(
`id` int AUTO_INCREMENT,
`title` varchar(100),
`body` varchar(5000),
`author` varchar(30),
`create_date` date,
primary key(`id`)
);

For running the app:
python app.py

# my web

need apache2 and mysql-server

create database

step 1
```
create user 'userz'@'localhost' identified by 'qwerty123';
grant all privileges on *.* to 'userz'@'localhost';
FLUSH PRIVILEGES;
```

step 2
```
mysql -u userz -pqwerty123;
create database data;
use data;
```

step 3
```
CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(50) NOT NULL,
  creation_time DATETIME NOT NULL
);
```

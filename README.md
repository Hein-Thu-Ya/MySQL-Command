# Data Definition Language (DDL)

## Show All Databases

```mysql
show databases;
```

## Choose Database

```mysql
use database_name;
```

## Create Database

```mysql
create database `db_name`;
```

## Delete Database

```mysql
drop database db_name;
```

## Create Database Table

```mysql
CREATE TABLE `table_name` (
    `id` INT UNSIGNED NOT NULL PRIMARY KEY AUTO_INCREMENT,
    `name` VARCHAR(200) NOT NULL,
    `email` VARCHAR(200) NOT NULL,
    `gender` CHAR(6) NOT NULL,
    `dob` DATE NOT NULL,
    `age` INT UNSIGNED
);
```

## Show Table from Database

```mysql
show tables;
```

## Show Columns from Table

```mysql
explain `table_name`;
describe `table_name`;
show columns from table_name;
```

## Delete Database Table

```mysql
drop table table_name;
```

<br><br>

# Data Manipulation Language (DML)

## Create Data

```mysql
INSERT INTO `table_name` (`name`, `email`, `gender`, `dob`, `age`) VALUES ("John Doe", "johndoe@gmail.com", "male", "1996-06-23", 30);
```

## Show Data / Select Data

```mysql
SELECT `id` `name`, `email`, `gender`, `dob`, `age` FROM `table_name`;

SELECT * FROM `table_name`;

SELECT * FROM `table_name` WHERE id = 1;
```

## Update Data

```mysql
UPDATE `table_name` 
SET `gender` = "male", `age` = 31
WHERE `id` = 3;
```

## DELETE Data

```mysql
DELETE FROM `students` WHERE id = 1;
```
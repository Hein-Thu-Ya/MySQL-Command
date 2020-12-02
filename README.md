# MYSQL Database Basic Command

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
CREATE TABLE `students` (
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
```

## Delete Database Table

```mysql
drop table table_name;
```
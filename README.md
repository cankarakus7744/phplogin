# PHP Login System

This is a simple PHP login system that allows users to register, log in, and log out. It uses MySQL for the database and sessions for user authentication.

## Features

- User registration with username and password
- User login with username and password
- User logout
- Session management to keep users logged in
- Password validation (Currently storing passwords in plain text. No hashing present.)


## Requirements

- PHP 7.0 or higher
- MySQL
- XAMPP or any other local server environment


## Usage

1. Locate "htdocs" directory of XAMPP.

2. Clone the repository or download the source code into said directory.
```bash
git clone https://github.com/cankarakus7744/phplogin.git
```

3. Start the XAMPP control panel and ensure that Apache and MySQL are running.

4. Navigate to "localhost/phpmyadmin/" in your browser and create a database named "database1".

5. Within "database1" create a table named "login":
```
CREATE TABLE `login` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `username` varchar(50) NOT NULL,
  `password` varchar(255) NOT NULL,
  PRIMARY KEY (`id`)
);
```
 >Database name has to be "database1". Otherwise change db_name inside of "connection.php" accordingly.

6. Navigate to "localhost/phplogin/" in your browser.

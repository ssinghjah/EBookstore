# EBookstore
A simple e-bookstore built using PHP, Apache, and SQL

- Clone this repo on a Linux machine
- Navigate within the folder of the cloned repo
- Run `sudo bash setup.sh` to install PHP, MySQL, and Apache and configure phpmyadmin. This script was tested on Ubuntu 20.04. Enter `Y` whenever prompted.
- Run `sudo mysql -u root`
- Add new user `CREATE USER 'csc547'@'localhost' IDENTIFIED by 'CsCEcE547@Cloud';`
- Grant all privileges to user `GRANT ALL PRIVILEGES ON *.* TO 'csc547'@'localhost' WITH GRANT OPTION;`
- Type `exit;`
- Setup the database by running `source databaseSetup.sql`
- Update the $servername, $username, and $password variables within products.php:
  - `$servername = "localhost";`
  - `$username = "csc547";`
  - `$password = "CsCEcE547@Cloud";`
- Copy `products.php` and `products.js` to `/var/www/html/`
- Open a browser and navigate to http://localhost/products.php to view the Bookstore app

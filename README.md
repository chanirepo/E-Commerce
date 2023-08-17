# E-Commerce

                                          E-Commerce Demo Project
# Take Ec2 Ubuntu server
# sudo su
# sudo apt update
# sudo apt upgrade
# sudo apt install php -y
# sudo apt install php8.1-fpm php8.1-curl php8.1-bcmath php8.1-mysql 
php8.1-xml php8.1-zip php8.1-gd php8.1-intl php8.1-pdo
# sudo apt install apache2 -y
# sudo apt install mysql-server
# sudo mysql_secure_installation
 enter y
 0
 Y
 n
 Y
 y
# Sudo mysql
 ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
 FLUSH PRIVILEGES;
 exit
# cd /var/www/html/
# rm index.html
# git clone your_git_repo
# mysql -u root -p
 password: password
 CREATE DATABASE ecommerce_marolix;
 show databases;
 exit
# cd /var/www/html/E-Commerce/database/database/
# mysql -u root -p ecommerce_marolix < ecommerce_marolix.sql
 password: password
# mysql -u root -p
 password: password
 show databases;
 use ecommerce_marolix;
 show tables;
 exit
# cd /var/www/html/E-Commerce/E-commerce-7June
# mv .env.example .env
# vi .env
 DB_CONNECTION=mysql
 DB_HOST=localhost
 DB_PORT=3306
 DB_DATABASE=ecommerce_marolix
 DB_USERNAME=root
 DB_PASSWORD=password
# cd ~
# php -r "copy('http://getcomposer.org/installer', 'composer-setup.php');"
# php composer-setup.php
# php composer.phar
# sudo mv composer.phar /usr/local/bin/composer
# composer
# sudo chown -R www-data:www-data /var/www/html/E-Commerce
# sudo chmod -R 775 /var/www/html/E-Commerce/
# cd /var/www/html/E-Commerce/E-commerce-7June/
# composer update
# composer install
# php artisan key:generate
# php artisan migrate
# sudo service apache2 restart
Go to browser http://localhost # ec2 puplic ip address
OutPut

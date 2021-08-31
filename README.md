1). Setup Database Credentials in .env
In this step, go to your project directory and open .env file and set your database credentials like this:

 DB_CONNECTION=mysql
 DB_HOST=127.0.0.1
 DB_PORT=3306
 DB_DATABASE=databasename
 DB_USERNAME=db_username
 DB_PASSWORD=db_password

2) Create Customers table in your defined database 

CREATE TABLE `customer`.`customer` ( `id` INT NOT NULL AUTO_INCREMENT , `name` VARCHAR(255) NOT NULL , `email` VARCHAR(255) NOT NULL , `contact_number` VARCHAR(255) NOT NULL , `updated_at` TIMESTAMP NOT NULL , `created_at` TIMESTAMP NOT NULL , PRIMARY KEY (`id`)) ENGINE = InnoDB;

3) Finally run the project by
 php artisan serve

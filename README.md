# Ecommerce-Rest-API

a rest api of an ecommerce application that was linked with a frontend with react js 

# Configure Database
Once MySQL is installed you must configure a username and password. By default the user and password should be root . If not, you must configure in the file application.configure located in the path src/main/resources/.

In the file application.configure you must edit the parameters spring.datasource.username and spring.datasource.password with the values you defined.

# Create Database & Tables
Now you just need to create the database where the project will store the information. To create it, just follow the steps below. 

- CREATE DATABASE ecommerce;

Now you can run the server which generates the database tables

Create admin user
Before continuing you must create the user admin, in order to perform administrator operations in the application. For this you must create a user on the MySQL monitor with the following command.

USE ecommerce;
INSERT INTO user (username, email, is_admin, password) values ('{admin.username}', '{admin.email}', true, '{admin.password}');

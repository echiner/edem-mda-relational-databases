# EDEM - MDA - Relational Databases

## Introduction

<img width="300" src="https://www.itvel.com/img/db_icon_sqlserver_oracle_mysql.jpg">

In this module we will learn how to create a database model, at different levels (logical and physical).
First (Exercise 1) we will create an Entity Relationship model, and then (Exercise 2) we will implement it creating the required tables in MySQL.

## Exercises

* [**Exercise 1**: Creating a Data Model](Exercise1)
* [**Exercise 2**: Implementing the Data Model](Exercise2)

## Understanding the components

For the second exercise we will be using a popular relational database (MySQL):

* **MySQL**: Open-source database, which will be the data source
* **Adminer (MySQL UI)**: Web-base front-end to brower and interact with the database

This is the config we have in the Docker Compose:

| Component | Ports | URL/Comments |
| ------------- | ------------- | ------------- |
| **MySQL** | 3306  | Host: mysql<br/>Credentials: mysqluser/mysqlpw  |
| **Adminer (MySQL UI)** | 8090  | http://localhost:8090/  |
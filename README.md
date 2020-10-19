# EDEM - MDA - Relational Databases

## Introduction

<img width="300" src="https://www.itvel.com/img/db_icon_sqlserver_oracle_mysql.jpg">

In these module we will learn how to create a database model, at different levels (logical and physical).

## Initial Setup

We will be using the Docker Compose in this root folder, so start the Docker Compose components:

```shell
docker-compose up -d
```

```shell
# List the running services
docker ps

# Stop a specific service
docker-compose stop <SERVICE>
```

## Services

You will find the services in the following URLs:

* [MySQL](http://localhost:8080/nifi)
* [Adminer](http://localhost:18080/nifi-registry)

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

## Shut down and destroy

```
# Shut down the cluster
docker-compose down
```
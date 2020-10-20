# Implementing the Data Model

## Introduction

In this exercise we will be creating the database based on the previous exercise. For this purpose, we will use the popular MySQL database.
We have also included a UI to easily browse it, but we highly recommend to do the exercise using the command line.

## Setup

Let first launch the database and the UI. In the root folder run the following:

```shell
docker-compose up -d
```

Now, connect to the database:

```shell
# Modify records in the database via MySQL client
docker-compose exec mysql bash -c 'mysql -u $MYSQL_USER -p$MYSQL_PASSWORD inventory'
```

And perform some basic queries in the MySQL screen:

```shell
# Switch to the "inventory" database (if not already in)
mysql> use inventory;

# List the tables
mysql> show tables;

# Query the "customers" table
mysql> SELECT * FROM customers;
```

Now take a look at the same using the UI: http://localhost:8090/

## Exercise

Now it is your turn. You will need to create the tables you defined in the Entity Relationship model for Exercise 1.

But first, let's create a separate database for it:

```shell
# Create the 
mysql> create database edem;
```

### Tips

* Create the tables in a TXT file first, and the run them one by one in the command line
* Beware of the execution order since there are dependencies due to Foreign Keys
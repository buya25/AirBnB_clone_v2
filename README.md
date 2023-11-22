# AirBnB Clone v2 Project

Welcome to the AirBnB Clone v2 project! This is an extension of the original AirBnB Clone project with additional features and improvements. Please follow the instructions below to set up and work with this codebase.

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Bug Free!](#bug-free)
4. [Console Improvements](#console-improvements)
5. [MySQL Setup - Development](#mysql-setup-development)
6. [MySQL Setup - Test](#mysql-setup-test)
7. [Delete Object](#delete-object)
8. [DBStorage - States and Cities](#dbstorage-states-and-cities)
9. [DBStorage - User](#dbstorage-user)
10. [DBStorage - Place](#dbstorage-place)
11. [DBStorage - Review](#dbstorage-review)
12. [DBStorage - Amenity... and BOOM!](#dbstorage-amenity-and-boom)

## Introduction

In the industry, you will often work on existing codebases. This project aims to simulate such scenarios by extending an existing AirBnB Clone codebase. Please follow the tasks listed below to enhance and add new features while maintaining the existing functionality.

## Getting Started

1. Fork this repository.
2. Clone your forked repository to your local machine.
3. Update the repository name to `AirBnB_clone_v2`.
4. Update the README.md with your information, but don't delete the initial authors.

## Bug Free!

Ensure that the codebase is bug-free and passes all unit tests. Use the following commands to run the tests:

```bash
python3 -m unittest discover tests 2>&1 /dev/null | tail -n 1
```

Make sure to run the tests with different storage engines as specified in the project requirements.

## Console Improvements

Update the `do_create` function in the `console.py` file to allow for object creation with given parameters. The syntax should be:

```bash
create <Class name> <param 1> <param 2> <param 3>...
```

Ensure proper handling of parameters, and don't forget to add tests for this new feature.

## MySQL Setup - Development

Write a script (`setup_mysql_dev.sql`) that prepares a MySQL server for the development environment. This script should create:

- A database `hbnb_dev_db`
- A new user `hbnb_dev` (in localhost)
- Set the password of `hbnb_dev` to `hbnb_dev_pwd`
- Grant all privileges on the database `hbnb_dev_db` to `hbnb_dev`
- Grant SELECT privilege on the database `performance_schema` to `hbnb_dev`

## MySQL Setup - Test

Write a script (`setup_mysql_test.sql`) that prepares a MySQL server for the test environment. This script should create:

- A database `hbnb_test_db`
- A new user `hbnb_test` (in localhost)
- Set the password of `hbnb_test` to `hbnb_test_pwd`
- Grant all privileges on the database `hbnb_test_db` to `hbnb_test`
- Grant SELECT privilege on the database `performance_schema` to `hbnb_test`

## Delete Object

Update the `delete` method in `FileStorage` to delete an object from `__objects` if it's inside. If `obj` is equal to `None`, the method should not do anything.

## DBStorage - States and Cities

Transition from `FileStorage` to `DBStorage` using SQLAlchemy. Follow the specified steps to update the codebase, create necessary attributes, and establish relationships between `State`, `City`, and other classes.

## DBStorage - User

Update the `User` class to work with `DBStorage`. Add necessary attributes and relationships.

## DBStorage - Place

Update the `Place` class to work with `DBStorage`. Add necessary attributes and relationships.

## DBStorage - Review

Update the `Review` class to work with `DBStorage`. Add necessary attributes and relationships.

## DBStorage - Amenity... and BOOM!

Update the `Amenity` class to work with `DBStorage`. Create a Many-To-Many relationship between `Place` and `Amenity` using a new table `place_amenity`.

Congratulations! You now have a new and improved AirBnB Clone with support for MySQL and SQLAlchemy. Feel free to explore the codebase, run tests, and make further enhancements as needed.

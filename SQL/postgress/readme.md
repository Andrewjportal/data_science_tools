---
date: w04d03
duration: 90
maintainer: kiwidamien
order: 10
title: Postgress
---

# Sample Lesson Plan

# Learning Objectives

* Able to connect to a local postgres database in python using Psycopg
* Able to create a cursor
* Able to use a cursor to iterate through a set of results
* Be able to commit changes to the database, or rollback to previous commit

# Instructor Notes

This lesson should follow **sql-intro**

This will probably be a full day. SQLAlchemy has been dropped in favor of psycopg (they both do very similar things, and SQLAlchemy is _slow_ when dealing with
Postgres). If in future we work with ORM (Object Relational Managers) such as those used by Django or Flask, it would be worth bringing it back. At the moment,
it serves as a distraction.

The notebooks are:

* [AWS Setup](curriculum/project-03/aws-setup)



* `00_pandas_and_psycopg.ipynb`:

  Uses the _local_ postgres database, and interacts with it via Python. This will probably take a while (maybe 60 - 90 minutes), as concepts such as cursors, commits and rollbacks are discussed.

* AWS Setup followup:

  This should be assigned as homework. Especially in larger cohorts, a pattern that makes sense is to have everyone follow these instructions at home, and have everyone that was successful take an extended coffee break while helping those that encountered issues with the installation. Probably allow 15 minutes to help people install this.

* `01_example_connecting_to_baseball.ipynb`:

  This is about 20 minutes. This basically ensures that they get some practice with some simple queries using the baseball dataset. They use this same dataset in challenge 9. Note this notebook is duplicated in the AWS lecture, if you want to use it there to demonstrate you have successfully setup the AWS notebook.

# Additional Resources

---
date: w06d04
duration: 75
maintainer: kiwidamien
order: 10
title: MongoDB Lab
---

# Sample Lesson Plan
- [Mongo Shell](mongo_shell.md) (15 minutes)
- [Mogno Lab](MongoLab_Student.ipynb) (60 minutes)

Note that a pair exercise is included. This pair exercise makes sense _after_ this lab has been completed.



# Learning Objectives

Students will be able to
- Install datasets from JSON files using the `mongoimport` shell command
- Do simple find queries with mongo shell
- Be able to connect python to to a mongo instance using PyMongo
- Do simple find queries with PyMongo
- Iterate through cursors to process results from Mongo in Python
- Be able to run aggregation pipelines from Python on mongo collections
- Be able to insert and delete records from a collection
- Be able to drop collections from a database

# Instructor Notes

This lesson has an emphasis on different ways of selecting data. A short introduction to the shell version of `mongo` in javascript is included. It isn't strictly necessary, and could be removed, but you will need to run the `mongoimport` commands in there to load the data. I have included it because it is needed to set up permissions in mongo on AWS (and serves as a nice way of checking if `mongod` is set up correctly). Still, try and get through the shell version quickly. It probably works best if you run the commands as a demonstration -- students take forever to type in commands. The exercises in the notebook are much more useful.

Installing mongodb on OSX is relatively easy -- especially with brew -- and has been assigned as something to do at home. The instructions also call for students to install the `pymongo` package using `conda`. If something isn't working, making sure they followed this step is the first thing to check.

The installation directory also includes instructions for setup on Ubuntu and AWS. AWS is tricky because you should also set up user permissions. Note that students are not expected to use AWS for this lab, but many of them will want to use mongo on AWS for their project 4 and/or passion project.

# Additional Resources
- Extra files in the installation directory for installing mongo on AWS, and accessing it remotely.
- Other JSON datafiles for experimenting with in the `data/` directory
- `TwitterAPI.ipynb` has some nice examples of using different aggregations. The `twitter` folder also shows how to setup TwitterAPI, and includes some notes on Twitter streaming. Instructions on getting the API key and using `.env` files are also included here

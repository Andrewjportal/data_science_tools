---
date: w03d05
duration: 10
maintainer: kiwidamien
order: 10
title: SQL Setup
---

# Sample Lesson Plan

- (10m) [SQL Intro and Setup](01_SQL_Intro_and_Setup.ipynb)    
This lesson should be given as a homework exercise. It gets students to install PostgreSQL on their local machine, as well as creating the databases and tables for them.

# Learning Objectives

Students will
- Install PostgreSQL on their local machines
- Gain motivation for choosing SQL instead of simply loading csv files in pandas

# Depends On

[Pandas Intro](https://github.com/thisismetis/dscurriculum_gamma/tree/6d1d024468980093a81e7137f83dd19bd9c14718/curriculum/project-01/pandas-intro)

[Intro to Command Line](https://github.com/thisismetis/dscurriculum_gamma/tree/6d1d024468980093a81e7137f83dd19bd9c14718/curriculum/project-01/command-line)

# Instructor Notes

This is a placeholder to remind instructors and students to set up SQL **prior** to the SQL intro day. The first notebook with instructions is in this project

This is probably a worksheet you want to come back to after doing some SQL. A common pain point in the curriculum is that students don't see the value of doing
SQL for their projects (or they see the value but think there are too many things to learn and that SQL can be picked up later). They are surprised when entering
the interview stage that there is a lot more emphasis on SQL than machine learning techniques. This notebook contains some motivation and differences between SQL
and Pandas, but it is probably good to reiterate this once they have seen some SQL in practice.

## Big changes

* The current version does not start with the students needing to know AWS. Instead we install PostgreSQL locally (similar to the way we teach MongoDB). We still show
how to install PostgreSQL on an AWS instance later on, but the focus here is getting them to use SQL quicker (and not tie the AWS stuff mentally with SQL).
* The current version creates the databases and the tables for them via an install file. Here the motivation is that the interviews, etc will mostly be on the select
statements. It is probably good to encourage students to write their schema out to a separate file, so that the creation of the database may be reproduced on different
instances or machines.

# Additional Resources

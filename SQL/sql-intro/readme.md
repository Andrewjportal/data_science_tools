---
date: w04d01
duration: 75
maintainer: kiwidamien
order: 10
title: SQL Intro
---

# Prerequiste

This lesson depends on PostgreSQL being installed, which is covered in the [SQL Setup lesson](https://github.com/thisismetis/dscurriculum_gamma/tree/master/curriculum/project-03/sql-setup). This is meant to be done as an at-home exercise. I would recommend dedicating the "break time" after pair problems to students that had trouble installing PostgreSQL locally. Allow 15 minutes for this break.

Not assigning this as homework may not add substantially to the time taken but leaves the more computer-literate students bored and frustrated.

# Sample Lesson Plan

* (45 m) [Lesson 2: Intro to SQL through Exercises](02_SQL_Exercises.ipynb) with [Solutions](02_SQL_Exercises_w_solutions.ipynb)
* (30 m) [Lesson 3: SQL Lab Questions](03_SQL_lab_questions.ipynb)    
Don't expect students to complete questions within the alloted time. You might want to add 15 minutes to walk through solutions or leave as exercises.

# Learning Objectives

Students should:
- Be able to run commands in the Postgres REPL
- Be able to run simple SELECT commands to query what is in the database, and filter records using WHERE
- Be able to run aggregations (GROUP BY), and filter groups using HAVING
- Be able to JOIN different tables, and know which type of join (LEFT, RIGHT, INNER, OUTER) is appropriate
- Be able to create a VIEW
- Explain and understand why VIEWs exist, and why adding columns to the dataframe is a bad idea

This lesson does **not** cover
- Getting the data from SQL into other formats (e.g. Python, Pandas, CSV). This is the focus of tomorrow's lecture

# Depends On

[SQL Setup](https://github.com/thisismetis/dscurriculum_gamma/tree/master/curriculum/project-03/sql-setup)


# Instructor Notes

## SQL as a Language
There is no formal description of SQL as a language in this lecture, it is built up by example. Formal descriptions are available (e.g. https://www.postgresql.org/docs/9.5/static/sql-select.html). I haven't found these descriptions to be useful when teaching, as students tend to fall in one of two camps:

1. Those with SQL experience. They tend to know about these documents, and complain when we make simplifications of them.
2. Those without SQL experience. There is a lot of nuance they don't pick up from the syntax alone (e.g. all columns appearing in a statement with `groupby` have to appear as an aggregate or as a named column in the groupby).

## SQL Series Structure
The former curriculum spent most of the day prior to this lecture setting up SQL on AWS. By eliminating this step, we are able to move exercises forward in the series.

In this lecture, students are working with getting results with Postgres. After walking through several example exercises together, they can continue with additional questions from [this worksheet](03_SQL_questions_lab.md).

In the next lecture in the SQL series, students will be connecting to Postgres on their AWS instances. There is also an optional lecture on using SQL window functions.


# Additional Resources

* [The formal PostgreSQL documentation](https://www.postgresql.org/docs/9.5/static/sql-commands.html)

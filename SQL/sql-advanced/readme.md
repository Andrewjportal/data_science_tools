---
date: w04d02
duration: 45
maintainer: kiwidamien
order: 10
title: SQL Advanced (optional)
---

# Sample Lesson Plan

1. (45 minutes) [Advanced SQL notebook](Advanced_SQL.ipynb)



## Learning Objectives

* Able to use group aggregates in calculations for each row in a Pandas DataFrame
* Able to use SQL and subselects to use group aggregates in calculations for each row on a TABLE/VIEW
* Able to use SQL window functions to use group aggregates in calculations for each row on a TABLE/VIEW
* Able to use SQL window functions for running totals.

# Instructor Notes

This is an optional lecture, designed to show students two methods for adding results based on calculations within a _group_ to every row of a dataset.

## Structure

The syntax for a window function is a little strange. To help ease the pain, I have made an analogy with the `pandas.DataFrame.transform` method.

The simplest type of calculation is when we use the _same_ value for the aggregate within each group. We present 4 ways of calculating the same quantity (two with Pandas, and two with SQL). Students are free to decide within the approaches which they prefer (i.e. which of the Pandas approches make sense to them, and which of the SQL approaches make sense to them). I am not trying to push a particular methodology here (and nothing in the notebook addresses performance, which should be checked for the dataset in question).

The four approaches are
1. Doing a `groupby`, `merge` the result to calculate an aggregate of the group . Then we can calculate the percentage of the group's salary each person has -- we need the actual salary (row info) and the total group's salary (aggregated info).
2. Use the `pandas.DataFrame.transform` method to do the same calculation as step 1.
3. Calculate the same thing as we did in step 1 using the SQL analog of "group by"/"merge" (i.e. `GROUP BY`/`JOIN`). Shows a subselect.
4. Final version, which shows the same calculation using a window function.

The remaining sections show window functions where the aggregated value within each group changes row by row (e.g. rank, cumuluative sum, et cetera). We will see these in window functions that include an ORDER BY clause within the window function. You may want to remind students that we accomplished the same thing in earlier exercises with a self-join. In earlier versions of the curriculum we used a self-join to calculate customer "sales to date".

# Additional Resources

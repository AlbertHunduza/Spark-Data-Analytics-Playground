# Spark-Data-Analytics-Playground

![Spark Logo](spark_logo.png)

Welcome to the Spark Data Analytics Playground project! In this project, we explore the fundamentals of distributed computing using Apache Spark. We will work with Resilient Distributed Datasets (RDDs) and DataFrames to perform various operations and gain insights from the data. Additionally, we'll manipulate a recommender dataset using Spark's transformations and actions.

## Table of Contents

- [Introduction to Spark](#introduction-to-spark)
- [Exercise 1: Apache Spark Basics](#exercise-1-apache-spark-basics)
  - [Part a) Basic Operations on RDDs](#part-a-basic-operations-on-rdds)
  - [Part b) Basic Operations on DataFrames](#part-b-basic-operations-on-dataframes)
- [Exercise 2: Manipulating Recommender Dataset with Spark](#exercise-2-manipulating-recommender-dataset-with-spark)
- [Conclusion](#conclusion)
- [Getting Started](#getting-started)

## Introduction to Spark

Apache Spark is a powerful open-source distributed computing framework that provides efficient and flexible processing of large datasets. It offers high-level APIs in languages like Python, Java, Scala, and R. Spark's core abstraction, the Resilient Distributed Dataset (RDD), enables fault-tolerant distributed data processing. RDDs can be transformed and actions can be performed on them to achieve various data processing tasks.

## Exercise 1: Apache Spark Basics

### Part a) Basic Operations on RDDs

We start with basic operations on RDDs. We have two lists of words, 'a' and 'b', and we'll perform various operations using Spark RDDs.

1. **Right Outer Join and Full Outer Join Operations**: We perform rightOuterJoin and fullOuterJoin operations between 'a' and 'b' lists of words. Check the [spark_da_playground.ipynb](spark_da_playground.ipynb) notebook for detailed solutions.

2. **Counting Character "s" Using Map and Reduce**: We count how many times the character "s" appears in all words from lists 'a' and 'b' using map and reduce functions.

3. **Counting Character "s" Using Aggregate Function**: We count how many times the character "s" appears in all words using the aggregate function.

### Part b) Basic Operations on DataFrames

We continue with basic operations, but this time on DataFrames using the 'students.json' dataset.

1. **Replacing Null Values in Column 'points'**: Null values in the 'points' column are replaced with the mean of all points.

2. **Replacing Null Values in Columns 'dob' and 'last name'**: Null values in columns 'dob' and 'last name' are replaced with "unknown" and "--", respectively.

3. **Formatting Dates in 'dob' Column**: Dates in the 'dob' column are converted into the DD-MM-YYYY format.

4. **Calculating Age**: A new column 'age' is created, containing the calculated age of all students.

5. **Updating Points Based on Standard Deviation**: Students with points greater than 1 standard deviation of all points have their points updated to 20.

6. **Creating a Histogram**: A histogram is created for the new points generated in the previous step.

## Exercise 2: Manipulating Recommender Dataset with Spark

In this exercise, we work with the movielens10m dataset, specifically the 'tags.dat' file. We use Spark transformations and actions to solve various tasks related to tagging sessions and frequencies.

1. **Separating Tagging Sessions**: Tagging sessions for each user are separated based on a 30-minute inactivity duration.

2. **Calculating Tagging Frequency**: The frequency of tagging for each user session is calculated.

3. **Calculating Mean and Standard Deviation of Tagging Frequency**: Mean and standard deviation of tagging frequency are calculated for each user.

4. **Calculating Mean and Standard Deviation Across Users**: Mean and standard deviation of tagging frequency are calculated across all users.

5. **Identifying Users with Mean Tagging Frequency**: Users with a mean tagging frequency within two standard deviations from the mean frequency of all users are identified.

## Conclusion

In this Spark Data Analytics Playground project, we've explored the fundamental concepts of distributed computing using Apache Spark. We've worked with RDDs and DataFrames to perform various operations and gain insights from data. Additionally, we've manipulated a recommender dataset to extract meaningful information. This project serves as an introduction to the power and flexibility that Spark offers for large-scale data processing.

## Getting Started

To dive into the exercises and solutions, refer to the [spark_da_playground.ipynb](spark_da_playground.ipynb) notebook in this repository. The notebook contains detailed code and explanations for all the tasks mentioned in the exercises.

For visual references, you can find the exercise images here:
- [Exercise 1 Part 1](part1.png)
- [Exercise 1 Part 2](part2.png)
- [Exercise 1 Part 3](part3.png)

Feel free to explore, experiment, and learn from the provided notebook. Happy Sparking!

For any questions or issues, please reach out to [alberthunduza1@gmail.com](mailto:alberthunduza1@gmail.com).

---
*Note: This README provides a high-level overview of the project. For detailed instructions and code, please refer to the [spark_da_playground.ipynb](spark_da_playground.ipynb) notebook.*

# SQL Errors: NULL Handling and Implicit Type Conversions

This repository demonstrates two common yet subtle errors in SQL: incorrect handling of NULL values and implicit data type conversions.  The code examples show how these errors can lead to incorrect or unexpected query results and how to correct them.

## Bug 1: Incorrect NULL Handling

The first example shows a common mistake in checking for NULL values.  A simple `WHERE` clause checking for `NULL` might not yield the intended results when dealing with columns defined as `NOT NULL`. The correct approach is to utilize `LEFT JOIN` to avoid this pitfall.

## Bug 2: Implicit Type Conversions

The second example showcases the pitfalls of implicit data type conversions.  Implicit conversions can lead to inefficiency and unexpected behavior. Explicit type casting using functions like `CAST` ensures that the comparison is done with the correct data types.

## Solutions

The provided solution demonstrates the correct methods for handling NULLs and performing explicit type conversions. The `bugSolution.sql` file contains the corrected versions of the SQL queries.

## Learning Points

* Always be mindful of how `NULL` values are handled in your queries.
* Explicit type casting is essential for clear, efficient, and portable SQL code.
* Consider the benefits of `LEFT JOIN` over `WHERE` clauses when dealing with potential `NULL` values in related tables.
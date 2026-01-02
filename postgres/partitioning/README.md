## What is partitioning?
Partitioning is a database technique that splits a large table into smaller, more manageable pieces called partitions based on a partition key.
Each partition stores a subset of the data, but the table is still accessed as a single logical table by applications.

## Why is it used?
Partitioning is used to improve query performance and manageability for large tables.
It allows the database to scan only relevant partitions (partition pruning), which reduces I/O and speeds up queries.

## One limitation
Choosing the wrong partition key can reduce or eliminate performance benefits.
Too many partitions can also increase management overhead and negatively impact write performance.

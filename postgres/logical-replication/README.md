## What is logical replication?
Logical replication replicates data changes at the logical level, meaning it replicates individual INSERT, UPDATE, and DELETE operations.
It allows selective replication of specific tables using publications on the primary and subscriptions on the replica.

## Why is it used?
Logical replication is used when flexibility is required, such as replicating only specific tables, performing database migrations, or sharing data with downstream systems.
It allows different schemas or database versions between the primary and the replica.

## One limitation
Logical replication does not replicate schema changes (DDL) automatically and is not designed for high availability failover.
It also has more overhead compared to physical replication.

## What is physical replication?
Physical replication copies the entire database from the primary server to a replica at the WAL (Write-Ahead Log) level. 
The replica is an exact byte-level copy of the primary database and stays in sync by continuously applying WAL records.

## Why is it used?
Physical replication is mainly used for high availability and read scaling. 
It allows read-only replicas and provides a standby database that can be promoted if the primary fails.

## One limitation
Physical replication replicates the whole database and does not allow selective table replication. 
The primary and replica must have the same database version and schema, which makes it less flexible for migrations or partial data sharing.
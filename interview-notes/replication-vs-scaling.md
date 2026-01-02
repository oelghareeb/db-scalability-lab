## When to use replication
Replication is used when high availability and fault tolerance are required.
It allows the system to continue serving traffic if the primary database fails and can also be used to scale read operations.

## When to use partitioning
Partitioning is used when a single database node holds large tables and query performance becomes an issue.
It improves performance by allowing the database to scan only relevant partitions instead of the entire table.

## When to use sharding
Sharding is used when a single database server cannot handle the data size or traffic volume.
It scales the database horizontally by distributing data across multiple nodes.

## Real-world examples

### Replication
An e-commerce application uses a primary database for writes and multiple replicas for reads to ensure high availability and reduce read latency.

### Partitioning
A logs or events table is partitioned by date (daily or monthly) to speed up queries and make old data easier to archive.

### Sharding
A large social media platform shards user data by user_id across multiple database servers to handle massive traffic and data volume.
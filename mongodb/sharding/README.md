## What is sharding?
Sharding is a database scaling technique that horizontally distributes data across multiple database servers (shards).
Each shard stores a subset of the rows based on a shard key, allowing the database to scale beyond a single node.

## Why is it used?
Sharding is used to scale databases horizontally by distributing data and query load across multiple servers.
A shard key allows the query router to direct requests to the correct shard, which improves performance and scalability.

## One limitation
Choosing a poor shard key can lead to uneven data distribution and hot shards.
Sharding also increases operational complexity, especially for cross-shard queries and rebalancing.

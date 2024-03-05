# Types of Partitioning

## Horizontal Partitioning (Sharding)

- The databases/tables are divided into partitions of rows, also called *shards*
based on a *range*

- That is, every time a shard grows beyond the range, the extra data is moved to
a new shard

- Therefore, all the shards/partitions have the same schema

- Hence, it is sometimes also called *range-based partitioning*

- However, it may lead to unbalanced/unequal partitioning of the database

## Vertical Partitioning

- The database is divided into partitions of tables/columnns i.e. different
partitions store different tables/columns

- Therefore, each shard will have a different schema

- However, this leads to slower join queries

- Sometimes we may need to partition even further if a column/table grows larger

## Directory-Based Partitioning

- Data is divided into various machines and a *directory server* is established
to keep the metadata

- That is, the directory server keeps the mapping of data and servers

- This promotes *loose coupling* b/w client and server and leads to high (horizontal)
scalability

- However, it is complex, which leads to difficulties in implementation

- The directory server may act as a single point of failure if it is not replicated

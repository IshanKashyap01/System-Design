# Replication

It refers to *copying of data* on multiple machines i.e. synchronizing multiple
machines

## Types of Replication

## Active Replication

Data is replicated on all nodes of the cluster

## Passive Replication

- It follows the **master-slave** architecture

- Therefore, all read-write operations are done on the *master* node

- While the data is replicated on all the *slave* nodes in an offline session

- If the *master goes down*, one of the *slave is promoted to master*

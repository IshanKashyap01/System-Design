# CAP Theorem

## What it Stands For

- The C stands for **Consistency** i.e. data consistency should be maintained

- A stands for **Availability** i.e. application should be available at all times

- P stands for **Partition tolerance** i.e. *network partitions* should be handled
well

### Network Partitions

- Network is one of the *most unreliable* thing in the world of distributed systems

- Due to n/w failures, we can have a node no longer in connnection with the rest

- This situation is known as **network partition**

## What it Means

- The CAP theorem states that in a distributed system, **only two of these three**
can be achieved at any time

- However, *partition tolerance* (fault tolerance) must be maintained at all times
as otherwise we may suffer a **huge data loss**

- Therefore, we always have to choose b/w *consistency* and *availability*

- This is because *strong consistency* leads to *low availability* and *high*
*availability* leads to *low consistency*

- However, if we don't choose *both* then we will have *low* replication and redundancy

- Consequently, any failure will cause severe harm to the application and its data

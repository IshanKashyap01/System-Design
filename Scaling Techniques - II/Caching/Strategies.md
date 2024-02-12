# Different Caching Strategies

## Write Through Cache

- Data is *simultaneously written* to the *database* and the *cache*

- Therefore, it *prevents stale data* and *increases read consistency*

- However, *write* operations will be *slower*

## Write Around Cache

- For each write operation, write is only performed once directly to the database

- Searching is done in the cache *first*, then the database, in case of a *cache*
*miss*

- If the cache search is a miss (*cache miss*), the data is loaded into the cache

- Then the cache returns the data to the client

- Therefore *write operation is fast* but the read is very slow in case of a miss

## Write Back Cache

- On a write operation, the cache is updated *first*, then the database is updated
in an offline session

- Therefore, write operations are very fast

- However, in case the cache fails, data can be lost

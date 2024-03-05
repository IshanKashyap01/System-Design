# Different Techniques of Partitioning

These techniques are used to decide which partition a data/record should be stored

## Hash-Based Partitioning

- It works like a `HashMap` as data is passed through a hash function to decide
where it will be stored

- However, adding new servers becomes problematic as it invalidates the hash function

- Every time servers are added/removed, data migration is required and during the
process, neither hash functions will be valid

- Therefore, it will cause a down time for the entire duration of the process

### Consistent Hashing

- The servers are assigned a virtual address by passing their IP addresses through
a hash function

- Data is passed through the same function and assigned to the *next* closest match

- Therefore, whenever servers are added/removed/down, data continues to persist

- Only the data stored in a wrong location is migrated while the remaining data
remains available

- `Cassandra` uses the consistent hashing technique for partitioning

## List Partitioning

- Data is classified into different keys and each machine contains a list of keys

- When data comes, it is sent to the server with a match for its key

## Round Robin Partitioning

- Data is stored to different partitions in a circular fashion

- That is, if the last data was stored in machine 1, the next will be stored
in machine 2

- This ensures even distribution of data

# Types of Consistency

## Strong Consistency

- It is achieved when we *stop* clients from *reading* data until all servers are
updated

- It is used in all *banking* and other *transactional* applications

## Eventual Consistency

- The system remains in an *inconsistent state* until *all nodes* are updated

- Therefore, some clients will get *stale data* until consistency is achieved

- All *social media* applications follow eventual consistency

## Weak Consistency

- It is the *worst* model of consistency as we don't ensure consistency at all

- Therefore, each node may contain different data at any point of time

# Indexing in Databases

- Tables in an RDBMS are stored in the sorted order of the primary keys

- Therefore, indexing is used when we have *read-intensive* non-primary key columns

- When we create an index, its content is copied into a separate location

- The data is stored along with the pointers to the original locations in a B-Tree

- Therefore, when a query requires a search on this column, it happens in this
index instead of the table

- Once the data is found, its pointer is used to get the corresponding row in the
table

## When to Use Indexing

- Indexing makes searching faster but it also takes up extra memory and leads to
maintainance overheads

- It speeds up *read* operations but also slows down *write* operations

- This is because the *write* operation will be performed on both the table and
the index

  - Depending on the data structure used, it operation can be pretty expensive

- Hence, it should *only* be used for *read-intensive* columns with large amounts
of data

- That is, only use it for the most searched, large column(s) in the database

- Using it on small tables may lead to more time spent on resolving pointers than
searching

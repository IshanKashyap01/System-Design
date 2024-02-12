# Types of Databases

## File-Based Storage Systems / File-Based Database Management Systems

Data is stored in files which are arranged into folders

### Disadvantages

1. Data duplication/redundancy is very high

2. Security is minimal

3. Only programmers can use it easily

4. Data retrieval is not very efficient

## Relational Database Management System (RDBMS)

It stores related data in the form of tables based on a strict schema

### Advantages

1. Data redundancy is avoided

2. Provides high security

3. Very simple to use through SQL queries

4. Data retrieval is very fast and efficient

5. Provides a more intuitive structure for storing data via relations and keys

### Challenges

1. Rigid schema

2. Less scalable

## NoSQL Databases

- It stores all kinds of data based on a dynamic/less strict schema

- It can store *structured, semi-structured and unstructured* data

### Scenarios for Usage

1. When the schema for the data changes dynamically

2. Data is in huge volume/velocity/veracity (big data)

3. There is no need for joins on tables

4. When data is non-relational

### Types of NoSQL Databases

1. Key-Value Databases

    - Generally used for caching, for example, Redis

2. Document-based Databases

    - Data is stored in a document format for ex. MongoDB (BSON)

    - It brings the best of both worlds (RDBMS & NoSQL)

3. Columnar Databases

    - Data is stored in the form of columns in the memory

    - Useful when we only want to query certain columns (analytics)

4. Graph Databases

    - Data is stored as nodes and interconnected via edges, for example, Google
Maps

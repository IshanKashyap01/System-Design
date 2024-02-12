# Introduction to Caching

- The goal of caching is to *improve read* by avoiding additional calculations

- It stores frequently used data in memory to avoid n/w and disk I/O, API calls
and other calculations

- It caches expensive static results (the same result for every call) into local
storage

## Example

- DB hits are often expensive and results are often (at least partially) static

- Therefore, frequently requested queries can be cached into the system

- Both front-end and back-end as well as browsers can cache data

## Types of Cache

### Application Server Cache

It caches frequently used but rarely changing data acquired from databases, APIs
and other heavy calculations

### Content Delivery Network (CDN) Cache

It caches static content and delivers it to the front-end

## When to Use

1. When data is not changing very frequently

2. If the application is **read intensive** i.e. read operations always outnumber
write operations. Ex. websites

## When Not to Use

1. When data changes frequently

2. If the application is write-intensive. Ex. highly interactive web apps

    - Here caching will prove to be an unnecessary overhead

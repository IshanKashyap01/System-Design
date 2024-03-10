# REST

- There can be two applications that needs to interact w/ each other but do not
share the same tech stack

- For ex. an application written in java may need to interact with one written
in C++, Python or JS

- Therefore we need a form of communication that serves the following requirements:

    1. Enable communication over a n/w

    2. Language independent

    3. Light-weight

    4. Fast

- The `REST` framework, which stands for *Representational State Transfer*,
fulfils all these requirements

- An application needs to expose `REST` APIs to let other apps connect with it

## REST API

- For an app to interact w/ another using REST APIs, it needs the following:

    1. A `URI` (Universal Resource Identifier) to locate the data

    2. `CRUD` operation(s) to use the data

- A URI is basically the address of the data like 127.0.0.1/app/api/v2/data

- REST API provides the following CRUD operations: `POST`, `GET`, `UPDATE` and
`DELETE`

- The point at which an API connects w/ a s/w is called an *API endpoint*

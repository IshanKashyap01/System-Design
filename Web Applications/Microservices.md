# Microservice Architecture

- Microservice architecture is an evolution of SoA with 100% independence b/w the
services

- In SoA, different services may interact with the same database, and therefore,
share a dependency

- In microservice architecture, even the database layer is broken such that each
microservice will have its own separate database layer

- Each microservice has different code and are deployed separately i.e. instead
of reusing code, we reuse microservices

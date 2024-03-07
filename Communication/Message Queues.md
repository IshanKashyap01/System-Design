# Message Queues

- A message queue uses a queue to store requests that can be retrieved in a FIFO
fashion

- In the message-based pattern:

    1. The clients making the requests are called **producers**

    2. The message queue is called **agent/broker**

    3. The servers serving the requests are called **consumers**

- For ex. `Kafka`, `RabbitMQ`, `ActiveMQ` etc.

## Use Cases

1. When there are too many requests to handle

    - It is used when the requests per unit time is greater than the response time
of the server

    - In such a case, the requests will remain in the queue until the server is ready
to take them

    - Therefore, the server can maintain its throughput without getting overloaded

2. When we want to implement eventual consistency

    - Another use case is when the server needs to notify/update multiple clients in
a time-insensitive manner

    - It will send the update to the queue, which will then notify all the clients
one-by-one

3. When we want to decouple the clients and servers

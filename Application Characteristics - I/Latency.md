# Latency

- Latency is the **round trip time** i.e. the time it took a request to reach its
destination and the response to get back

- It differs from **response time** in the sense that it doesn't account for compuation
time in the server

$$
\text {Response time =  Latency +  Compuation time}
$$

- Basically, latency refers to the *delays* in the system

## Latency Based on Architecture

- Latency is *high* in systems with *higher network usage/dependency*

- Therefore, *monolithic* systems will always have *lower* latencies in comparison

## How to Improve Latency

- Latency can be improved by decreasing **network delays**

- One way to do it can be done to improve *network bandwidth*, however it is *expensive*

- We can use **Content Delivery Network**, which allows multiple servers to host
the same data

- Another factor is **computational delays** that can be caused by busy servers

- *Load balancing* or *parallelism* on the servers can help *minimize* this delay

- We can also use *caching* to serve requests faster

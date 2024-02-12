# Load Balancing Algorithms

## Round Robin Method

- The load balancer will *sequentially* serve requests to all available servers

- This strategy works when all servers have *equal capacity*

### Weighted Round Robin Method

- This algorithm considers the *capacity of each server* for work distribution

- Hence, *traffic distribution is in proportion to server capacities*

- This strategy works well even when servers have *varying capacities*

## IP Hash Algorithm

- It is used when servers have almost the *same capacities*

- It does a *random*, *unbiased distribution* of traffic

- It passes the IP address of the client through a *hash function*

- The returned value denotes the *server* that will get the request

## Least Connection Algorithm

- It is used when we need to decide on the basis of *open connections* on a server

- In other words, it sends request to the server with *least number of connections*

## Least Response Time Algorithm

- It is used to *minimize response time*

- It sends requests to the server with the *least response time*

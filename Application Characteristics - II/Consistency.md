# Consistency

- A *consistent* application returns the *same response* for the *same request*
**every time**

- In a distributed system, we have many servers connected via a network so it takes
time to update data in all of them

- If during an updation process some clients access different servers, they'll get
different responses

- The clients accessing updated server will get the latest response

- While others will get **stale information** also known as **dirty read**

- To maintain consistency at all times, servers should *prohibit reads* until
*all servers are updates*

## Consistency and Architecture

- *Monolithic* systems are natively consistent as there is only one point of data
access

- However, *distributed systems* need extra measures to ensure consistency due to
*redundancy and replication*

## Factors Impacting Consistency

- It depends on how fast we can *update replicas* i.e. nodes are *properly synchronized*

- Moreover whether or not are we in a position to stop *read*

## Factors Improving Consistency

- We should *stop read* while updating replicas

- By *improving bandwidth* we can update all servers quicker

- Strategies for choosing replicas should consider the *distance b/w them*

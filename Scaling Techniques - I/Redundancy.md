# Redundancy

- It is used in the *context of nodes (server/computer) or components*

- That is, redundancy is the duplication of nodes

- Therefore, if one node fails, the clients can rely upon other nodes

- This phenomena is called **failure recovery/management**

## Types of Redundancy

### Active Redundancy

All nodes will be served requests by a load balancer

### Passive Redundancy

- Only a few nodes will actively serve requests while the others will act as backups

- Therefore, iff an active node breaks, the passive will replace it

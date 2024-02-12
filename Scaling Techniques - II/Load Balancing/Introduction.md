# Load Balancer

## Responsibilities of a Load Balancer

1. Ensure *each server is equally loaded*

2. Health check (checks for available nodes)

3. Maintain *high* throughput and availability

## When to Use

When you have multiple instances of the same application

- Suppose front-end, back-end and database are all scaled to multiple systems

- Each layer can have a dedicated load balancer

## When Not to Use

1. When you're using a *monolithic* architecture on a single system

2. When your app is present on a *single* vertically scaled system

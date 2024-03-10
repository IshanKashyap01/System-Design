# Server Oriented Architecture (SoA)

- In SoA, applications are kept as granular as possible and let them interact
over a n/w

- The client is known as a **service requester** whereas the server is known as
the **service provider**

- Similarly to a client-server architecture, a service/app can act as either

## Advantages

- Easy to selectively scale the application

- Time taken to update is less as services are more granular

- Devs are free to choose different tech stacks for different services

- Development teams can be much bigger, as each can work on different components
or services

- Enforces loose coupling

## Challenges of SoA

- Additional n/w calls increases latency of the system

- Testing is difficult due to continuous changes/additions to the system

- Security is more complex to enforce due to different tech stacks used

- Can be confusing for developers new to the architecture

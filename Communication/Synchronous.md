# Synchronous Communication

- In synchronous communication, the client keeps waiting until the server responds
to its request

- It is also known as a **blocking call**

- It keeps the *design simple* but also *tightly couples* the client and the server

- It is used whenever transactions or real-time decision making are required

- For ex. maintaining consistency, payments, reservations, sequential applications,
troubleshooting etc.

- A communication session is established by both the client and the server

- Then the requesting thread is blocked (kept in waiting) until a response

- Such a step is called a **blocking step**

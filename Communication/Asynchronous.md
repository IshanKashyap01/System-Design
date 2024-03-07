# Asynchronous Communication

- In asynchronous communication, the client receives a tracking ID and moves on
to other tasks instead of waiting

- The client will then hit the server again with the tracking ID to check if a
response is generated or not

- It is also called as a **non-blocking call** and **start/stop** communication
as start/stop bits are used as a means of timing the data being sent

- Therefore, it allows the decoupling of components so they can work independently

- It makes the system more scalable if we make all the non-essential communication
asynchronous

## Use Cases

- It is generally used when the response calculation takes a lot of time

- If a client can make requests faster than the server can respond, it'll lead
to cascading failure of the entire system

- In such a case, asynchronous communication is needed to keep the application
running

- For ex. booking confirmation, quarterly/monthly transaction reports from banks,
emails, social media etc.

## How Asynchronous Communication Works

1. Request-response pattern / tracking ID based pattern

    - The client makes a request and receives a tracking/job ID from the server

    - The client will keep checking with the server after regular intervals

    - While the server continues the job and the requesting thread keeps doing
    other tasks

2. Message queue based communication

    - Instead of sending the request directly to the server, it is sent to a
    queue as a message

    - The server picks these messages from this queue and performs its job

    - Once it finishes its process, it will notify the client in some way

    - It could be **peer to peer (P2P)**, where *each message has only one receiver*

    - Or, it could follow a **publish subscribe model** where a message is sent
    to *multiple receivers*

# Communication Protocols

## Pull Model

- In the pull model, also called **Polling**, the request is driven by the client

- It is the more commonly used paradigm for communication

- It is useful whenever the requested data can be readily served to the client

- If in the push model, the server has to keep track of too many clients, this
model should be used

## Push Model

- In the push model, server pushes the data to the client w/o the client asking
for it

- It is useful when the client has to request multiple times before the data is
made available and sent to it

## Long Polling

It is a short-lived connection where the server waits until either the data is
ready, in which case the response can be delayed or the request times out

## Socket Connection

- It is a two-way communication useful when the client and server communicate
frequently w/ each other

- It establishes a long-lived duplex connection channel based on the TCP protocol

## Server Sent Events (SSE)

- It is a long-lived, one-way connection channel that the server uses to gradually
send data as it is calculated

- The client will have to open another channel to make requests to the server

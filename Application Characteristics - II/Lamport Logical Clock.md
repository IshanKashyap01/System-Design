# Lamport Logical Clock

- Developed by *Leslie Lamport* in 1978, it is used for finding the order of events
in a distributed system

- It provides a partial order of events

## Algorithm of Lamport Logical Clock

- Each process uses a local integer counter initialised to zero

- When an event occurs, this counter is incremented

- The counter is assigned as a timestamp for each event

- A send event carries its own timestamp/counter while a receive event is calculated
as:

$$
\text {receive time = MAX(local time, send time + 1)}
$$

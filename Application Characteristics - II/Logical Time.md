# Importance of Logical Time

## Problems in Using Physical Clock in Distributed Systems

1. There's no concept of a global physical time

2. Problem in finding the precise order of events

3. Network delays can change the original sequence of events

## Logical Local Time

- Carries information about events *within* the system

- Uses a process that marks its own events and a protocol to update after each
regional event

## Logical Global Time

Stores local knowledge about the logical global time and uses a protocol to
update when processes exchange data

# Event Sourcing

Event Sourcing is a way of storing the state of an application. Instead of saving just the current state, it saves all the events that happened to cause the state to change. This way, the complete history of changes is stored.

## How it Works
- Every time something changes in the system, an event is created. These events are saved in an append-only log, meaning new events are added, but old ones are never changed.

## Why Use It
- You can look back at all the events and replay them to figure out how the system got to its current state.
- This helps with  finding and fixing problems and checking what happened.

## Benefits
- It makes it easier to understand how the system works by keeping a full history of all changes.
- It helps with complex processes and keeps everything consistent, especially in systems that have many different parts.

## Challenges
- Storing all events can require a lot of space.
- If the events change over time , you have to be careful about how you handle these changes.
- Rebuilding the state from the events can take a lot of resources, so using  saving the state at certain points can help.

## Final Thoughts
- Event Sourcing gives a  reliable and way to track how things change over time. It helps keep systems flexible and resilient.



Reference site :- https://martinfowler.com/eaaDev/EventSourcing.html?utm_source

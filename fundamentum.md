Fundamentum
===========

The foundation for elos core server stack.

#### Requirements

##### Server
 * Database connection
 * Model system
 * Websocket connection system
 * Websocket connection protocol

##### Data
 * User model (id, token, name, events)
 * Event model (start time, end time, title, user)

##### App
 * N/A

#### Resolution

Elos runs a [go server](https://github.com/elos/server) that connects to a [mongo database](https://github.com/elos/server). We have a user model and event model. Web socket communication is fully functional with a broadcast system based on channels and concerns[*].

* an article still needs to be written describing this behavior

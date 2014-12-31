Dawn
----

The first elos project. Dawn is a mobile app that interacts with elos' main server, recording events. Specifically, dawn records the start and stop times of an event along with the "event's" name. The application will be written for iOS, and will be native swift code.

#### Requirements
-----------------
##### Server
 * Support of a websocket connection
 * Running live on elos.io

##### Data
 * User model and event model

##### Client
 * Login
 * Create account(?)
 * Start event
 * Name event
 * Stop event

##### Testing
 * Server database infrastructure
 * User model and event model
 * Hub infrastructure

##### Documentation
 * Need to document core server architecture decisions: hub and concerns
 * Testing with go

#### Progress
-------------
##### Server
- [ ] Project costs of running elos server
- [ ] Decide where to host elos
- [ ] Decide if separate host for go server and mongo
- [ ] Decide if nginx is overkill at this point
- [ ] Get builds of the elos server
- [ ] Get binary of elos server running on remote virtual host
- [ ] Get mongo db running on remote virtual host
- [ ] Get go server talking to mongo db on remote virtual host
- [ ] Get go server responding to external requests

##### Documentation
- [x] Write article on [data-centric nature of elos](https://github.com/elos/ideation/blob/master/functionality/data.md)
- [ ] Write on elos' concern model of data

##### Testing

#### Resolution
---------------

[Elos' is Data-Driven](https://github.com/elos/ideation/blob/master/functionality/data.md)

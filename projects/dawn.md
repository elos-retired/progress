Dawn
----

The first elos project. ~~Dawn is a mobile app that interacts with elos' main server, recording events. Specifically, dawn records the start and stop times of an event along with the "event's" name. The application will be written for iOS, and will be native swift code.~~ The app was cancelled. Dawn primarily consisted of elos infrastructure buildig, including running elos on a digital ocean instance.

#### Requirements
-----------------
##### Server
 * Support of a websocket connection
 * Running live on elos.io

##### Data
 * User model and event model

##### Client [CANCELLED]
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
- [x] Project costs of running elos server
- [x] Decide where to host elos
- [x] Decide if separate host for go server and mongo
- [x] Decide if nginx is overkill at this point
- [x] Get builds of the elos server
- [x] Get binary of elos server running on remote virtual host
- [x] Get mongo db running on remote virtual host
- [x] Get go server talking to mongo db on remote virtual host
- [x] Get go server responding to external requests
- [x] Don't [override model if unauthenticated or already created](https://github.com/elos/server/issues/1) (namely posting a user's id)

##### Documentation
- [x] Write article on [data-centric nature of elos](https://github.com/elos/ideation/blob/master/functionality/data.md)
- [x] Write on elos' [concern model of data](https://github.com/elos/documentation/blob/master/data/concerns.md)

##### Testing
- [x] All of util package except logging utilities
- [x] Autonomous client data agent
- [x] data/transfer package
- [x] Routing, both config/routes & the routes package
- [x] Models: user, event

#### Resolution
---------------

* [Digital ocean](https://www.digitalocean.com) appears to be the highest quality cheap hosting option.
* Digital ocean's lowest [pricing level](https://www.digitalocean.com/pricing/) is $5/month for 1 core and 512mb of RAM. This should suffice for now.
* We will run mongo locally with the go server for now
* nginx is overkill right now
* Building the server is fine, but it funky because of mongo dependency and system deps. You have to build for linux on a linux box.
* Decided not to use a binary but instead just use the git repo, set up a fresh server with setup.sh.
* [Elos is Data-Driven](https://github.com/elos/ideation/blob/master/on/data.md)
* Elos manages its distribution of data with model [concerns](https://github.com/elos/documentation/blob/master/data/concerns.md)


##### This project was declared finished on 3/22/15.
 * Server tasks handled.
 * App cancelled


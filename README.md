#Bank 
This application is an project created to improve my Scala knowlage

# Architecture
Bank application
* each bank account is a persistent actor
* all events are recorded (creation, update etc)
* all events are replayed in case of failure/restart
* one big bank (persistent) actor manages all actors
* a HTTP server with REST API handles requests
* all events are stored in Cassandra

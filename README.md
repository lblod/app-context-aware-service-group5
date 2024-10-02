# app-context-aware-service-group5

Service bootstrapped using a mu.semte.ch microservices environment.

### Hooking things up with docker-compose

The `docker-compose.yml` file is alters so it contains all microservices of the framework together with
the context-aware-service and context-aware-frontend modules as containers.

### Configure the dispatcher

The file `config/dispatcher/dispatcher.ex` is altered to add a route between the frontend and the backend service as well 
as to route incoming traffic on the identifier to webserver serving the static web page.

### Boot up the system

Boot your microservices-enabled system using docker-compose.

    cd /path/to/app-context-aware-service-group5
    docker-compose up

You can shut down using `docker-compose stop` and remove everything using `docker-compose rm`.

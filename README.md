# great-expectations-template
Standardized directory structure and resources for development of  Great Expectations projects


## Requirements
A docker runtime with support for docker-compose.


## How To Use
All command line examples assume a *nix environment.

### Initial Repo Setup
Create a new git repo using this repo as a template.

Clone your new git repo and update/remove the LICENSE as appropriate to your use case.

### Booting The Development Environment
```
# cd ~your new repo~/runtime`
# docker-compose up`
```
At this point you should have a running docker container which has mounted ~your new repo~/project and ~your new repo~/data into the container at /home/project and /home/data respectively.

Note: docker-compose was chosen as a way to codify the boot process to ensure a consistent and trouble free startup. It is not strictly necessary for the development environment to function as intended. For example the same result is possible using only the docker command syntax. See runtime/docker-compose.yml to understand the required configuration for booting using the docker command syntax.


more info here about the container booting in attached mode to the cli and being able to access the container
$ docker exec -it ge-dev bash

### Initializing Your Project

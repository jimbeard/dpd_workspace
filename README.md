# Demo Docker / Python stack

This demo comprises the following two repos, which should be cloned into a common parent directory:-
1. https://github.com/jimbeard/dpd_workspace
    - contents:-
        - nginx service (entry point / load balancer)
        - project configuration (docker .env, docker-compose.yml, shared volume)
1. https://github.com/jimbeard/dpd_data_loader
    - contents:-
        - example data loader service


## Pre-requisites

1. install Docker Desktop
1. install VS Code and the Microsoft / VS Code Docker extension

## Setup:-

1. create a parent directory\
```> mkdir docker_python_demo && cd docker_python_demo```
1. clone the two repos into this directory
    1. workspace
        - no further action needed
    1. data-loader
        - follow the steps in the data-loader project README.md to make sure it runs as a stand-alone application

1. open the main docker-compose.yml
    - right-click in the IDE edit window and select 'Compose Up' from the context menu
    - this should build images of the source components and start them in containers in Docker Desktop
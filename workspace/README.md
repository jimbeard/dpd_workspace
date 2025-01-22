# Demo Docker / Python stack

This demo comprises the following three components which should be cloned into a common parent directory:-
1. nginx
1. data-loader
1. workspace


## Pre-requisites

1. install Docker Desktop
1. install VS Code and the Microsoft / VS Code Docker extension

## Setup:-

1. create a parent directory\
```> mkdir docker_python_demo && cd docker_python_demo```
1. clone the three 'docker python demo' projects into this directory
    1. nginx
        - no further action needed (this is just a proxy config)
    1. data-loader
        - follow the steps in the data-loader project README.md to make sure it runs as a stand-alone application
    1. workspace
        - no further action needed (this is just a 'wrapper' config for the above components)

1. open the main docker-compose.yml
    - right-click in the IDE edit window and select 'Compose Up' from the context menu
    - this should build images of the source components and start them in containers in Docker Desktop
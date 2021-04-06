# data_science_neo4j_docker
Docker template for basic data science packages to interface with Neo4j

## Introduction

This container is based on the Juptyer data science container along side creating a Neo4j database on your local machine. This container does NOT include support for GPU-based deep learning packages (that will be a separate repo).  There are a lot of Python packages in this container that you might not use and so this container might be a bit bloated.  It is more of a generic container to get you started.

## To run this container

At the CLI within this folder:

```
docker-compose up
```

When you are done with the container, stop it vial `CTRL-c` and then:

```
docker-compose down
```

## Some notes

- There are two different Python packages that can be used to connect to Neo4j from within Python.  It is probably easiest to just pick one and go with it.
  - `[neo4j]`(https://neo4j.com/docs/api/python-driver/current/): The official, Neo4j-supported Python driver
  - `[py2neo]`(https://py2neo.org/2021.0/): A community-developed driver with lots of solid documentation and examples out there

# data-warehouse-etl

ETL Data Warehouse Testing and Data Quality Management using Postgres 

## Getting started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

## Prerequisites

- [Docker](https://www.docker.com/products/docker-desktop) (required*)

## Installing

Step by step instructions on how to get a working version of the project on your local machine:

```
$ git clone <repo>
$ cd ./<repo>
```

> `docker-compose up` 

This will fetch the latest [postgres docker image](./docker-compose.yml). On start-up it will copy and run the [init scripts](./scripts/pgsql_init/) to setup a DB called `postgres` with a `public` schema. The [data folder](./scripts/data/) is copied to the container and the scripts will insert the data into the postgres DB. 
In the section pgadmin, Instead of having to download and install pgAdmin and Postgres on your machine, this process provides a quick and easy way to get things set up. 
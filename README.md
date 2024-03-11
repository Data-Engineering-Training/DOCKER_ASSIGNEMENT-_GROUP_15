# PostgreSQL Docker project

## Group Members 

* 1. FRANCISCA FRIMPOMAA AMPONSAH
* 2. Ishmael Abayateye Kabu
* 3. ANGEL ADAAMBIIK
* 4. ERIC AKWETE AJAVON
* 5. PETER KOBENA EDUAH



## Requirements:
* docker >= 17.12.0+
* docker-compose

## Quick Start
* Clone or download this repository
* Go inside of directory,  `cd postgres-docker-project`
* Run this command `docker-compose up -d`


## Environments
This Compose file contains the following environment variables:

* `POSTGRES_USER` the default value is **postgres**
* `POSTGRES_PASSWORD` the default value is **setyourpassword**
* `PGADMIN_PORT` the default value is **5050**
* `PGADMIN_DEFAULT_EMAIL` the default value is **pgadmin4@pgadmin.org**
* `PGADMIN_DEFAULT_PASSWORD` the default value is **admin**

## Access to postgres: 
* `localhost:5432`
* **Username:** postgres 
* **Password:** setyourpassword 

## Access to PgAdmin: 
* **URL:** [http://localhost:5050](http://localhost:5050)
* **Username:** pgadmin@pgadmin.org 
* **Password:** admin 

## Add a new server in PgAdmin:
* **Host name/address** `postgres`
* **Port** `5432`
* **Username** as `POSTGRES_USER`, by default: `postgres`
* **Password** as `POSTGRES_PASSWORD`, by default `setyourpassword`


## Logging

There are no easy way to configure pgadmin log verbosity and it can be overwhelming at times. It is possible to disable pgadmin logging on the container level.

Add the following to `pgadmin` service in the `docker-compose.yml`:

```
logging:
  driver: "none"
```

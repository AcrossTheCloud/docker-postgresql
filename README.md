## PostgresSQL Dockerfile


This repository contains **Dockerfile** of [PostgreSQL](https://www.postgresql.org/) for [Docker](https://www.docker.com/).

### Installation

1. Install [Docker](https://www.docker.com/).

### Build
```shell
docker build -t="yourdockerusername/postgresql" github.com/acrossthecloud/postgresql
```

### Usage

#### Run `postgresql`

    docker run -d -p 27017:27017 --name postgresql matthewberryman/postgresql

#### Run `postgresql` w/ persistent database directory

    docker run -d -p 27017:27017 -v <db-dir>:/var/lib/postgresql --name postgresql matthewberryman/postgresql

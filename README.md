# Test task "Naveksoft"

Create docker-compose.yml and and the scripts it needs.

Docker-compose do:
  - runs clickhouse-server and clickhouse-client in containers;
  - creates database analytics and table events at first launch;
  - on the first launch after creating the analytics.events table, several events are put there for the test;
  - after restarting the container, the table is not cleared.

## Installation

Install Docker Engine guide: [Docker Engine](https://docs.docker.com/engine/install/ubuntu/)

Install Docker Compose guide: [Docker Compose](https://docs.docker.com/compose/install/)

## Usage

```docker
docker-compose up -d
```
File "create_database.tsv" contains queries for creating a database, creating and filling the table.

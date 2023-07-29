# Postgres Docker Template

A template for docker-compose, folder setup and configuration for Postgresql. The project uses:

-   [Postgresql](https://hub.docker.com/_/postgres)
-   [pgAdmin](https://www.pgadmin.org/)

The versions aren't fixed and will pull the latest by default.

## Folders

### `import`

This is bound to the postgresql folder `var/lib/postgresql/import` so any datasets or backups can be easily copied into the container.

### `pgadmin`

Contains a pre-configured servers.json for pgAdmin. This has setup a group and added the postgresql server as an entry.

### `postgres-data`

This binds all the postgresql data to persist the data.

## Getting started

1. Modify any of the environment variables
2. Replicate any changes in the servers.json
3. Run `docker-compose up -d`

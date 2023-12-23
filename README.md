# task-manager

## Backend

list http://localhost:5000

## Database PostgreSQL

```bash
CREATE DATABASE taskmanager;
CREATE USER taskmanager;
ALTER USER taskmanager WITH ENCRYPTED PASSWORD '123123';
GRANT ALL PRIVILEGES ON DATABASE taskmanager TO taskmanager;

\q
```

### set new schema

```bash
psql --username=taskmanager

CREATE SCHEMA taskmanager;
```

## for docker

```bash
docker run --name postgres-taskmanager -p 5432:5432 -e POSTGRES_PASSWORD=123123 -d postgres

TYPEORM_CONNECTION=postgres
TYPEORM_USERNAME=postgres
TYPEORM_PASSWORD=123123
TYPEORM_DATABASE=postgres
TYPEORM_PORT=5432
```

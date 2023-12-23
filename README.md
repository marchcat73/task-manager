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

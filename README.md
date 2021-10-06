# Postgresql sample database

Init database:
```bash
docker-compose up postgres
```

Connect to database with `postgres` user:
```bash
psql -h 127.0.0.1 -U postgres -d postgres
```

Create database `dvdrental` once you are logged in:
```SQL
CREATE DATABASE dvdrental;
```

Use pg_restore binary to load data on the freshly created `dvdrental` database:
```bash
pg_restore -h 127.0.0.1 -U postgres -d dvdrental dvdrental.tar
```

https://www.postgresqltutorial.com/load-postgresql-sample-database/

Connect to dvdrental database and have fun!
```bash
psql -h 127.0.0.1 -U postgres -d dvdrental
```

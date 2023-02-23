### Postgres-sql

#### Docker: Database
- Create a container running postgres-14:`docker run -e POSTGRES_PASSWORD=lol --name=pg --rm -d -p 5432:5432 postgres:14`.
- Directly to postgres: `docker exec -u postgres -it pg psql`.
- Check for commands for postgres to navigate through the database: HELP `\?`.
- Create your database to work from `CREATE DATABASE name` then switch to it `\c name`.
- Postgres with node: `https://node-postgres.com`.
#### Docker: JSONB
- Create  a new container `docker run -e POSTGRES_PASSWORD=lol --name=sql -p 5432:5432 -d --rm btholt/complete-intro-to-sql`.
- Run postgres: `docker exec -u postgres -it sql psql`.
- Javascript language extension for postgres used for stored procedures: `https://plv8.github.io`.
#### Movie Database
- Run the same container`docker run -e POSTGRES_PASSWORD=lol --name=sql -d -p 5432:5432 --rm btholt/complete-intro-to-sql`.
- Run postgres: `docker exec -u postgres -it sql psql omdb`.
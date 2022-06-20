## Run postgres within docker container

```bash
docker run --name some-postgres -p 5432:5432 -e POSTGRES_PASSWORD=mysecretpassword -d postgres
```

**Open it in an interactive shell**

```bash
docker exec -it some-postgres bash
```

- change to user ‘postgres’ \
  `su postgres`

- run the psql \
  `psql`

- list all databases \
  `\l`

- Create a database \
  `CREATE DATABASE "student";`

- Connect to "student" db \
  `\c student`

- Check connection info \
  `\conninfo`

- quit \
  `\q`

## Run postgres within docker container

```bash
docker run --name some-postgres -p 5432:5432 -e POSTGRES_PASSWORD=mysecretpassword -d postgres
```

**Open it in an interactive shell**

- change to user ‘postgres’
  su postgres

- run the psql
  psql

- check databases
  \l

- check connection info
  \conninfo

- quit
  \q

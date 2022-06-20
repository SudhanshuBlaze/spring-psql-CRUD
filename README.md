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
  
- show all relations \
  `\d` 
  
- Schema of the relation "student"
  `\d student`

- Create a database \
  `CREATE DATABASE "student";`
  
- Grant user privileges
  `GRANT ALL PRIVILEGES ON DATABASE "student" TO postgres;`

- Connect to "student" db \
  `\c student`

- Check connection info \
  `\conninfo`

- quit \
  `\q`

### User postgres user
`$ sudo -i -u postgres`

### Enter into postgres
`$ psql`

### Exit postgres
`$ \q`

### Create new user (after switching to postgres user)
`createuser --interactive`
`$ sudo adduser <username>`

Once this new account is available, you can either switch over and connect to the database by typing:
```
$ sudo -i -u sammy
psql
```

### Create new database
`$ createdb <dbname>`

### Commands within psql
```
\list or \l: list all databases
\dt: list all tables in the current database using your search_path
\dt *.: list all tables in the current database regardless your search_path
```

### Create table example
```
CREATE TABLE playground (
    equip_id serial PRIMARY KEY,
    type varchar (50) NOT NULL
);
```
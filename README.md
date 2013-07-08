App-migrate
===========

Easily migrate your database.

#Set up

`migrate install`

The setup process creates a very simple table in your database to maintain
records of the migrations. The table looks as below:

`CREATE TABLE db_migrate_tiny (version INT PRIMARY KEY)`

#Migrate to latest migration

`migrate latest`

##Mgrate to a specific version

`migrate to VERSION`

#Generate new migration

`migrate generate NAME`

By default, migrations are generated in `migrations` directory. You can also
pass `--dir` option to specify a directory.
